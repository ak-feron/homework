node {
    docker.image('golang').inside {
        stage('Build') {
            sh 'make build'
        }

        stage('Test') {
            sh 'make test'
        }
    }
    //def customImage = docker.build("my-image:${env.BUILD_ID}")
    //customImage.push()
}
