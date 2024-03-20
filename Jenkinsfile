pipeline {
    agent any
    triggers {
        GenericTrigger(
            ...
            genericVariables: [
                [key: 'main', expression: '$.ref', expressionType: './jason']
            ],
           // token: 'mySecureToken',
            ...
        )
    }

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
                sleep(time: 1, unit: 'SECONDS') // Added parameters for clarity
                echo 'I\'m ok'
            }
        }
        stage('Push Artifact') {
            steps {
                script {
                   
                    //git config user.email "your_email@example.com"
                    //git config user.name "Your Name"
                    //sh 'echo "Hi" >> file6'

                    //this command is run
                    bat 'echo "Hallo Welt"'
                    //this command is not run 
                    sh 'echo "Hallo Welt"'

                     //git add file5000
                    // git commit -m "Add artifact"
                    //git push origin main
                    //sh 'git clone https://github.com/nima3608/jenkinss.git'
                   
                    //THIS COMMAND RUN UND CLONE GIT IN C:\programdata\jenkins\.jenkins\workspace\Jenkinsfil_github_simple 
                    //git url: 'https://github.com/nima3608/building-a-multibranch-pipeline-project.git', branch: 'main'
                    
                }
            }
        }
    }
}
