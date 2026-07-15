pipeline {
    agent any

    tools {
        terraform 'terraform'
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Terraform Check & Init') {
            steps {
                echo 'Checking Tools...'
                sh 'terraform version'
                sh 'terraform init'
            }
        }
    }
}
