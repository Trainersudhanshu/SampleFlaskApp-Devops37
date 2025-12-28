pipeline {
    agent {
        label 'ec2'
    }

    stages { //stages =- "collection of jobs/stage/task == pipeline"
        stage("Run Docker Container"){ //job6
            steps{
                sh "docker rm -f webos"
                sh "docker pull jinny1/sampleflaskapp-devops37:latest"
                sh "docker run -d -it --name webos -p 80:80 jinny1/sampleflaskapp-devops37:latest"
        }
        }
        stage("succesfull deployment"){ //job7
            steps{
                echo "Application Deployed Successfully"
        }
        }
    }
}
