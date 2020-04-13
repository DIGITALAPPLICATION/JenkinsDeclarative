
pipeline{
    agent any
    
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
