pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git credentialsId: '57cf86b3-fe3d-4937-9333-39536263c90f', url: 'git@github.com:UmeshIndra123/Devops_CI_CD.git'

            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Add your deployment commands here
            }
        }
    }
}
