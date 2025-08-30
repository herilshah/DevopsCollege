pipeline {
    agent any
    tools { nodejs "Node 20" } 
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
                sh 'npm run build'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test -- --watchAll=false'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying React App...'
            }
        }
    }
}
