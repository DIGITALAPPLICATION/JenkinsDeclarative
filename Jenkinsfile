pipeline {
    agent any
    tools{
        maven 'maven-3.6.3' // make sure this is configured in Manage Jenkins --> Global Tool Configuration
    }
    stages {
        stage('Example') {
            steps {
                    git branch: 'sample', credentialsId: 'jenGit', url: 'https://github.com/DIGITALAPPLICATION/WebApp.git'
                    sh 'mvn -V clean install'
            }
        }
    }
}
