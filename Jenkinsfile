pipeline {
    agent any
    stages {
        stage('Example') {
          agent { docker 'maven:3-alpine' } 
              steps {
                  sh 'mvn -v'
            }
        }
        stage('Example Test') {
            agent { docker 'openjdk:8-jre' } 
            steps {
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
}
