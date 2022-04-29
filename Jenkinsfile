pipeline {
    agent any
    tools {nodejs "node"}
    stages {
        stage('Example') {
      steps {
        sh 'npm config ls'
      }
    }
        
        stage('Build') {
            steps {
                git 'https://github.com/kaushik-code/simple-node-js-react-npm-app.git'
                sh 'npm install --dry run'
                sh 'npm install'
                sh 'export NODE_OPTIONS=--openssl-legacy-provider'
                sh 'npm run build'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
}
