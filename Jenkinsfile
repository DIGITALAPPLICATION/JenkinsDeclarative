pipeline {
	agent any
	stages {
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
