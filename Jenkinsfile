pipeline {
    agent any

    stages {
        stage('Terraform Check') {
            steps {
                echo 'Checking Tools...'
                sh 'terraform version'
                sh 'terraform init'
            }
        }
    }
}
