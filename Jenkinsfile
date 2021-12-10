pipeline {
    agent any

    tools {
        maven "jenkins-maven"
    }

    stages {
        stage('Git Checkout') {
            steps {
                git 'https://github.com/sudeepranjan/sample-webapp.git'
            }
        }
        
        stage("Test Stage"){
            steps{
                echo "test stage..."
            }
        }
        
        stage("Maven Build"){
            steps{
                bat 'mvn clean package'
            }
        }
    }
}
