pipeline {
    agent {
        docker {
            image 'golang'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'make build'
            }
        }
        stage('Test') {
            steps {
		sh 'make test'
            }
        }
    }
}
