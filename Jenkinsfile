pipeline {
	agent any
	triggers {
		//Execute weekdays every four hours starting at minute 0
		cron('0 */4 * * 1-5')
		//Query repository weekdays every four hours starting at minute 0
		pollSCM('1 * * 1-5')
		//Execute when either job1 or job2 are successful
		upstream(upstreamProjects: 'job1, job2', threshold: hudson.model.Result.SUCCESS)
	}
	stages {
		stage('trigger-example'){
			steps{
				echo "Run some script"
			}
		}
	}
}
