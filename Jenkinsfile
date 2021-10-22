pipeline {
    agent any
    stages {
        stage('Example') {
           steps { bat "exit 0" }
        }
    }
    post { 
	failure {
	   mail body: 'Hi Naresh', subject: 'The Pipeline failed', to: 'naresh@gmail.com'
        }
    }
}
