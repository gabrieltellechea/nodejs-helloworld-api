pipeline {
    agent any
    tools {
        nodejs 'nodejs'
    }
    stages {
        stage('ClonarRepo') {
            steps {
                sh 'git clone https://github.com/gabrieltellechea/nodejs-helloworld-api.git'
          }
        }
        stage('Build') {
            steps {
                echo "Ejecutar npm install" 
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo "Ejecutar npm test push" 
                sh 'npm test'
            }
        }
    }
}
