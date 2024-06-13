pipeline {
    agent any

    triggers {
        cron('H/2 * * * *')
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout code from the repository
                git branch: 'main', url: 'https://github.com/nima3608/jenkinss.git'  
            }
        }
        stage('Build') {
            steps {
                echo 'Building......'
                // Add your build steps here
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test steps here
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deployment steps here
            }
        }
    }
}

