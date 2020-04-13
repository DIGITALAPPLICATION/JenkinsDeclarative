
pipeline{
    agent any
    
    parameters{
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
    }
    
    stages{
        
        stage('simple'){
            steps{
                
                println "declarative"
                
                
                sh 'echo hi '
                
                script{
                    def sam = "yes"
                    if(sam == "yes"){
                      echo 'yes'
                    }else {
                      echo 'no'
                    }
                }
            }
        }
    }
}
