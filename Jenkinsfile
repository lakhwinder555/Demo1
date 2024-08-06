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
            steps {
                echo 'Deploying...'
                
            }
        }
        stage('Email Notifications') {
            steps {
                    mail bcc: '', body: '''email notificatoin sent 
                    thanks''', cc: '', from: '', replyTo: '', subject: 'jenkinsjobs', to: 'lakhwindersinghwins@gmail.com'
            }
        }
    }
}
