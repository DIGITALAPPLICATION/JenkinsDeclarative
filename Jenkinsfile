pipeline {
    agent any

    stages {
        stage('Example') {
            steps {
                
                    withCredentials([[$class: 'UsernamePasswordMultiBinding', credentialsId: 'jenGit', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD']]) {
                        sh 'echo uname=$USERNAME pwd=$PASSWORD'
                    }
                
            }
        }
    }
}
