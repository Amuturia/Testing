pipeline {
    agent {
        label 'nodejs' 
               
    }

    tools {
        nodejs 'nodejs-22.3' 
                //This is the first time am working with the tools part.
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Amuturia/gallery'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
      
    }
    
    // I trying this for a change. Might be useful, might not. One way to know is try it out.
    post {
        always {
            echo 'Pipeline finished.'
        }
        success {
            echo 'Pipeline succeeded.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
