pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
		stage('Test') {
            steps {
                bat 'npm run dev'
            }
        }
        stage('Deliver') {
            steps {
				bat'npm run build'
            }
        }
    }
}
