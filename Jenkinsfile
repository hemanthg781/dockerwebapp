node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerlogin') {

        def customImage = docker.build("hemanthg781/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
