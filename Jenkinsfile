pipeline {
    agent any
    stages {
        stage('Example') {
           steps { "test" }
        }
    }
    post { 
	failure {
	   mail body: 'Hi Naresh', subject: 'The Pipeline failed', to: 'naresh@gmail.com'
        }
    }
}
