pipeline {
    agent any
    tools{
        maven 'maven-3.6.2' // make sure this is configured in Manage Jenkins --> Global Tool Configuration
    }
    stages {
        stage('Example') {
            steps {
                    sh 'mvn -v'
            }
        }
    }
}
