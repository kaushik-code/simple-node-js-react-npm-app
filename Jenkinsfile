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
                sh 'npm i npm@6.14.4'
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
