pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Add build steps here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add test steps here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add deploy steps here
            }
        }
        stage('Email Notification') {
            steps {
                    mail bcc: '', body: '''email notificatoin sent 
                    thanks''', cc: '', from: '', replyTo: '', subject: 'jenkinsjobs', to: 'lakhwindersinghwins@gmail.com'
            }
        }
    }
}
