pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
            when {
                branch 'staging'
            }
            stage('Email notification') {
                mail bcc: '', body: '''Hi Welcome to Jenkins Email Notification 
                 Thanks''', cc: '', from: '', replyTo: '', subject: 'jenkinsjob', to: 'lakhwindersinghwins@gmail.com'
            steps {
                echo 'Deploying to staging... 1234'
            }
        }
    }
}
