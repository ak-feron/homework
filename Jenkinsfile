node {
    def customImage = docker.image('golang').inside {
        stage('Build') {
            sh 'make build'
        }

        stage('Test') {
            sh 'make test'
        }
    }

    customImage = docker.build("hello-app")

    docker.withRegistry('http://178.63.61.82:5000') {
        customImage.push()
    }
}
