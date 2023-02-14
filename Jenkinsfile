pipeline {
  agent any
    stages {
        stage('Build') {
            steps {
              script {
                sh 'g++ first.cpp'
                echo 'Build Stage Successful'
              }
                
            }
        }
        stage('Test') {
            steps {
              script {
                sh './a'
                echo 'Test Stage Successful'
              }
                
                
            }
        }
        stage('Deploy') {
            steps {
              script {
                echo 'Deployment Successful'
              }
                
            }
        }
    }

    post {

        failure {
            echo 'Pipeline failed'
        }
    }
}
