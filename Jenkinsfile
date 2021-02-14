pipeline {
    agent {
    docker {
        image 'node:6-alpine'
        label 'my-defined-label'
        args  '-p 3000:3000 -p 50000:50000'
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
