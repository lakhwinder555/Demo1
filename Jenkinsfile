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
         stage('Email Notification') {   
                mail bcc: '', body: '''email notificatoin sent 
                thanks''', cc: '', from: '', replyTo: '', subject: 'jenkinsjobs', to: 'lakhwindersinghwins@gmail.com'
            }    
            steps {
                echo 'Deploying to staging... 1234'
            }
           
        }
    }
 }
