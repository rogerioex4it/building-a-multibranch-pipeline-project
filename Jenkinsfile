pipeline {
    agent {
    docker {
        image 'node:6-alpine'
        label 'master'
        args  '-p 3000:3000'
    }
    }
    environment { 
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
    }
}
