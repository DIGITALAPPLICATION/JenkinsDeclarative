pipeline {
	agent any
	stages {
		stage ('checkout') {
			steps{
				git credentialsId: 'jenGit', url: 'https://github.com/DIGITALAPPLICATION/WebApp.git'
			}
		}
		stage ('Deploy stage') {
			when {
				branch 'master'
			}
			steps {
				echo 'Deploy master to stage'
			}
		}
	}
}
