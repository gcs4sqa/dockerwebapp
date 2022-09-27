node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("gcs4sqa/dockerwebapp:${env.BUILD_NUMBER}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
