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
        success {
            mail bcc: '', body: '''Hi Welcome to Jenkins Email Notification 
            Thanks''', cc: '', from: '', replyTo: '', subject: 'jenkinsjob', to: 'lakhwindersinghwins@gmail.com'
        }
    }
}

