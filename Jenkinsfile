pipeline {
    agent any

    environment {
      AWS_ACCESS_KEY_ID     = credentials('aws-secret-key-id')
      AWS_SECRET_ACCESS_KEY = credentials('aws-secret-access-key')
    }

    stages {
      stage('Deploy') {
          steps {
            terraform init .
          }
      }

      stage('Destroy') {
          steps {
            terraform init .
          }
      }   
    }
}
