node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'goldbuild-dockerhub') {

        def customImage = docker.build("goldbuild/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
