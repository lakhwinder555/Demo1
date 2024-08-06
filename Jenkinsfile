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
            steps {
                echo 'Deploying to staging... 1234'
            }
        }
    }
    post {
        always {
            stage('Email Notification') {
                steps {
                    mail bcc: '', body: '''Email notification sent 
                    Thanks''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job Notification', to: 'lakhwindersinghwins@gmail.com'
                }
            }
        }
    }
}
