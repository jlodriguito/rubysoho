pipeline {
    agent { docker 'ruby' }
    stages {
        stage('build') {
            steps {
                sh 'ruby --version'
            }
        }
        stage('test') {
            steps {
                sh 'ruby web.rb'
            }
        }
    }
}
