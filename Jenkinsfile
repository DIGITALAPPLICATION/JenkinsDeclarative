pipeline {
    agent any
    parameters {
        string(name: 'User', defaultValue: 'DevOps', description: 'Hello world')

        text(name: 'Demo', defaultValue: '', description: 'Demo parameter')

        booleanParam(name: 'Boolean', defaultValue: true, description: 'Boolean value')

        choice(name: 'CHOICE', choices: ['A', 'B', 'C'], description: 'Choose one')

        password(name: 'PASSWORD', defaultValue: 'Key', description: 'Enter a password')

    }
    stages {
        stage('Example') {
            steps {
                echo "Hello ${params.yyyyy}"

                echo "Biography: ${params.Demo}"

                echo "Toggle: ${params.Boolean }"

                echo "Choice: ${params.CHOICE}"

                echo "Password: ${params.PASSWORD}"
                
                sh '''
                    echo sample data into file line 1 > FILE.txt
                    echo sample data into file line 2 >> FILE.txt
                '''
                
                script{
                    if (fileExists("${env.WORKSPACE}/FILE.txt")) {
                        echo 'Yes, file created in Jenkins workspace'
                        def data = readFile "${env.WORKSPACE}/FILE.txt"
                        println(data)
                    } else {
                        echo 'No, file may not created in Jenkins workspace'
                    }
                }
            }
        }
    }
}
