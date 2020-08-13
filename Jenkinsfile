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
    //customImage.push()
}
