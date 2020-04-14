pipeline {
    agent any
    options {
        timeout(time: 30, unit: 'MINUTES')
        //retry(3)
    }
    stages {
        stage('Example') {
            agent{
                   label 'linux'
            }
            steps {
                echo 'Hello World'
            }
        }
    }
}
