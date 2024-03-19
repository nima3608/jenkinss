pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Bye') { // Corrected "By" to "Bye"
            steps {
                echo 'Bye World'
            }
        }
        stage('OK') {
            steps {
                sleep(time: 5, unit: 'SECONDS') // Added parameters for clarity
                echo 'I\'m ok'
            }
        }
        stage('Push Artifact') {
            steps {
                script {
                    sh '''
                    git config user.email "your_email@example.com"
                    git config user.name "Your Name"
                    git add path/to/artifact // Replace with your actual file path
                    git commit -m "Add artifact"
                    git push origin main
                    '''
                }
            }
        }
    }
}
