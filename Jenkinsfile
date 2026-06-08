pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                echo 'Testing Email'
            }
        }
    }

    post {
        always {
            emailext(
                subject: "Jenkins Email Test",
                body: "Email notification is working successfully.",
                to: "samatgworld@gmail.com"
            )
        }
    }
}