pipeline {
    agent any 
        
    stages{
        stage('BUILD and RUN'){
            steps{
                script{
                   sh "docker build . -t webserver"
                    sh "docker run -p 8000:80 -d webserver"
                }
            }
        }
    }
}
