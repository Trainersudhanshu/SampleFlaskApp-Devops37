pipeline {
    agent {
        label 'ec2'
    }

    stages { //stages =- "collection of jobs/stage/task == pipeline"
        stage("Run Docker Container"){ //job6
            steps{
                sh "docker pull jinny1/sampleflaskapp-devops37:latest"
                sh "docker run jinny1/sampleflaskapp-devops37:latest"
        }
        }
        stage("succesfull deployment"){ //job7
            steps{
                echo "Application Deployed Successfully"
        }
        }
    }
}
