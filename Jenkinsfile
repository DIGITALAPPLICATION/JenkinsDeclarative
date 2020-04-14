pipeline {
      agent any
      stages {
        stage('Run Tests') {
          parallel {
            stage('Test On Windows') {
              
              steps {
                sh "echo run-tests.bat"
              }
            }
            stage('Test On Linux') {
              
              steps {
                sh "echo run-tests.sh"
              }
            }
          }
        }
      }
    }
