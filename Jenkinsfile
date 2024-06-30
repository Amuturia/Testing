pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
            }
        stage('Verify Node.js and npm') {
            steps {
                sh 'node -v && npm -v'
            }
                
            }
        
    }
}

