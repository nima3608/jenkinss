pipeline {
    agent any

    tools {
        maven 'Maven 3.9.6' // Name der Maven-Installation in der Global Tool Configuration
    }

    stages {
        stage('Build') {
            steps {
                script {
                    // Setzen des Maven-Home-Pfads, falls erforderlich
                    env.MAVEN_HOME = tool name: 'Maven 3.9.6', type: 'maven'
                }
                // Führen Sie den Maven-Befehl aus
                sh 'mvn clean package'
            }
        }
    }
}

