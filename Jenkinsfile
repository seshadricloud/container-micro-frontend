pipeline {
    agent any 
    stages {
        stage("build"){
            steps {iii
                script {
            sh """
	    aws ecr get-login-password --region sa-east-1 | sudo docker login --username AWS --password-stdin 315073111691.dkr.ecr.sa-east-1.amazonaws.com
	    sudo docker build -t frontend .
	    sudo docker tag frontend:latest 315073111691.dkr.ecr.sa-east-1.amazonaws.com/frontend:latest
	    sudo docker push 315073111691.dkr.ecr.sa-east-1.amazonaws.com/frontend:latest

            """              
                }
            }
            
        }

    }
}
