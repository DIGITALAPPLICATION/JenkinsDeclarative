pipeline {
    agent any
    tools{
        maven 'maven-3.6.2' // make sure this is configured in Global Tool Configuration
    }
    stages {
        stage('Example') {
         	steps {
               		sh 'mvn -v'
            }
        }
    }
}
