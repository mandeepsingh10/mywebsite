pipeline {
    agent any 
        
    stages{
        stage('BUILD and RUN'){
            steps{
                script{
                    image = docker.build("mandeepsingh10/webserver")
                    sh "docker run -p 8000:80 -d mandeepsingh10/webserver"
                }
            }
        }
    }
}
