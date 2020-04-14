pipeline {
    agent any
    parameters {
	choice(
	    choices: ['QA' , 'PROD'],
	    description: '',
	    name: 'REQUESTED_ACTION'
	    )
    }

    stages {
	stage ('QA') {
	    when {
		// Only say hello if a "greeting" is requested
		expression { params.REQUESTED_ACTION == 'QA' }
	    }
	    steps {
		echo "Deployment for QA will be executed"
	    }
	}
	stage ('PROD') {
	    when {
		// Only say hello if a "greeting" is requested
		expression { params.REQUESTED_ACTION == 'PROD' }
	    }
	    steps {
		echo "Deployment for PROD will be executed"
	    }
	}
	   
    }
}
