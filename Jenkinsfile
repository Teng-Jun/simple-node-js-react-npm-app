pipeline {
    agent {
        docker {
            image 'node:14'  // Using Node.js 16 Docker image
            args '-u root:root'  // Run as root if necessary
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
                sh 'npm run build'  // Assuming you have a build script
            }
        }
    }
}
