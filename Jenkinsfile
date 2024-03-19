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
                   
                    //git config user.email "your_email@example.com"
                    //git config user.name "Your Name"
                    echo "Hi" >> file50
                    git add file50
                    git commit -m "Add artifact"
                    git push origim main
                    //sh 'git clone https://github.com/nima3608/jenkinss.git'
                   
                    //THIS COMMAND RUN UND CLONE GIT IN C:\programdata\jenkins\.jenkins\workspace\Jenkinsfil_github_simple 
                    //git url: 'https://github.com/nima3608/building-a-multibranch-pipeline-project.git', branch: 'main'
                    
                }
            }
        }
    }
}
