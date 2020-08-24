node {
    checkout scm

    docker.withRegistry('https://hub.docker.io/','dockerhub') {

        def customImage = docker.build("karthikaram/dockerize-jenkins-node-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}