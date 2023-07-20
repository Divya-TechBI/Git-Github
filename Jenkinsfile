pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
    post {
        always {
            emailext body: "A Test Email", recipientProviders: [[$class: 'DevelopersRecipientProvider']], subject:"Test", from: "jenkins@iSOCRATES.com", to: "divya.nn@isocrates.com", attachLog: true
        }
            
    }
}
