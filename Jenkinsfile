pipeline {
	agent any
	parameters {
		string(name: 'USER', defaultValue: 'DevOps', description: 'A user that triggers the pipeline')
	}
	stages {
		stage('Trigger pipeline') {
			steps {
				echo "Pipeline triggered by ${params.USER}"
			}
		}
	}
}
