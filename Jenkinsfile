node {
    checkout scm

    docker.withRegistry('https://index.docker.io/v1/','dockerhub') {

        def customImage = docker.build("karthikaram/dockerize-jenkins-node-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}