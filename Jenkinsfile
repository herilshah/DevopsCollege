pipeline {
    agent any

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
                // Later we can add Docker/Server/Netlify/S3 deployment
            }
        }
    }
}
