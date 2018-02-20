pipeline {
    agent { docker 'ruby' }
    stages {
        stage('build') {
            steps {
                docker build -f /root/docker/Dockerfile
            }
        }
        stage('test') {
            steps {
                sh 'ruby web.rb'
            }
        }
    }
}
