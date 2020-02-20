node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'sat-dockerhub') {

        def customImage = docker.build("sonuthestar/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
