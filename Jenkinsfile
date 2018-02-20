pipeline {
    agent { 
	docker {
		image 'rubuild:latest' 
		args  '-v /var/lib/jenkins/workspace/pipetest:/app'
		}
	}
    stages {
        stage('build') {
            steps {
               sh 'bundle'
            }
        }
        stage('test') {
            steps {
                sh 'ruby web.rb'
            }
        }
    }
}
