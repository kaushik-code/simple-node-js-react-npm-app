pipeline {
    agent {
        any {
             tools {
                 nodejs "nodejs"
             }
            image 'node:latest-alpine'
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}
