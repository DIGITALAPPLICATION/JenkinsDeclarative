pipeline {
    agent any
    parameters {
        string(name: 'User', defaultValue: 'DevOps', description: 'Hello world')

        text(name: 'Demo', defaultValue: '', description: 'Demo parameter')

        booleanParam(name: 'Boolean', defaultValue: true, description: 'Boolean value')

        choice(name: 'CHOICE', choices: ['A', 'B', 'C'], description: 'Choose one')

        password(name: 'PASSWORD', defaultValue: 'Key', description: 'Enter a password')

        file(name: "FILE.txt", description: "file to upload")
    }
    stages {
        stage('Example') {
            steps {
                echo "Hello ${params.yyyyy}"

                echo "Biography: ${params.Demo}"

                echo "Toggle: ${params.Boolean }"

                echo "Choice: ${params.CHOICE}"

                echo "Password: ${params.PASSWORD}"
                script{
                    if (fileExists('FILE.txt')) {
                        echo 'Yes, file uploaded to Jenkins workspace'
                        def data = readFile "${env.WORKSPACE}/FILE.txt"
                        println(data)
                    } else {
                        echo 'No, file may not uploaded to Jenkins workspace'
                    }
                }
            }
        }
    }
}
