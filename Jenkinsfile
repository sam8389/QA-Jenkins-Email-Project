pipeline {
    agent any

    post {
        always {
            emailext(
                subject: "Jenkins Email Test",
                body: "Congratulations! Jenkins email notifications are working.",
                to: "samatgworld@gmail.com"
            )
        }
    }
}