pipeline {
    agent any 

    stages {
        stage('Stage 1: Get Code from Git') {
            steps {
                git url: 'https://github.com/anilkumarsahu2623/my-jenkins-pipeline1.git', credentialsId: 'anilkumarsahu2623'
            }
        }

        stage('Stage 2: Print Message and Sleep') {
            steps {
                script {
                    echo 'Hello, you are in Stage 2'
                    sleep(time: 2, unit: 'SECONDS')
                }
            }
        }

        stage('Stage 3: Deploy Application') {
            steps {
                echo 'Deploying the application...'
                // Add deployment commands here
            }
        }
    }

    environment {
        MY_CREDENTIALS = credentials('anilkumarsahu2623')
    }
}
