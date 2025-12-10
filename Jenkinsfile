pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Build started..."
                echo "Build completed!"
            }
        }
    }

    post {
        always {
            emailext (
                subject: "Build Completed: ${env.JOB_NAME} #${env.BUILD_NUMBER}",
                body: "The build finished successfully!\nCheck the console at ${env.BUILD_URL}  this is nofief Email and our Ids is 20226148 and 20226147",
                to: '20226148@stud.fci-cu.edu.eg'
            )
        }
    }
}
