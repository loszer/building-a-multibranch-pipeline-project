pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 30001:30001'
        }
    }
    stages {
        stage('Build') {
            steps {
                echo '草，这么卡的么'
                echo "------"
                sh "node -v"
                sh "npm -v"
                echo "------"
                sh "npm config set registry http://r.cnpmjs.org"
                sh "npm install"
            }
        }
    }
}
