pipeline {
      agent none
      stages {
        stage('Run Tests') {
          parallel {
            stage('Test On Windows') {
              agent { label "windows" }
              steps {
                bat "run-tests.bat"
              }
            }
            stage('Test On Linux') {
              agent { label "linux" }
              steps {
                sh "run-tests.sh"
              }
            }
          }
        }
      }
    }
