pipeline {
    agent {
        docker {
            image 'golang'
        }
    }
    stages {
        stage('Build') {
            steps {
                make build
		make test
            }
        }
    }
}
