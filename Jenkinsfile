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
                sh "npm install --registry=https://registry.npm.taobao.org"
            }
        }
    }
}
