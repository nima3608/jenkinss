pipeline {
    agent any

    tools {
        maven 'Maven 3.9.6' // Name der Maven-Installation in der Global Tool Configuration
    }

    stages {
        stage('Build') {
            steps {
                // Führen Sie den Maven-Befehl aus
                bat 'mvn clean package'
            }
        }
    }
}

