
    pipeline {
        agent any
        stages {
            stage('Example') {
                steps {
                    echo 'Hello World'
                }
            }
        }
        post { 
            always { 
                echo 'Running after the stages in all the cases'
            }
            success { 
                echo 'Running after the stages only if success'
            }
            failure { 
                echo 'Running after the stages only if failed'
            }
        }
    }
