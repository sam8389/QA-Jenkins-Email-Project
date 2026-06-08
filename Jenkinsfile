pipeline {
    agent any

    tools {
        maven 'Maven'
    }

    stages {

        stage('Build and Test') {
            steps {
                bat 'mvn clean test'
            }
        }
    }

    post {
        always {
            archiveArtifacts artifacts: '**/surefire-reports/*'
        }
    }
}