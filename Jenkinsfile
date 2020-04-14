pipeline {
    agent any
    options {
        timeout(time: 1, unit: 'MINUTES')
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
