  GNU nano 4.8                                                                                                                 Jenkinsfile                                                                                                                           
pipeline {
    agent any
    environment {
        // Define environment variables here (optional)
        MY_ENV_VAR = 'value'
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Bhosales23/Exam.git'
            }
        }

        stage('Run Script') {
            steps {
                // Run your script )
                script {
                    sh './date_time.sh'

                }
            }
        }
    }

    post {
        always {
            echo 'This will always run after the pipeline finishes.'
        }
        success {
            echo 'This will run if the pipeline is successful.'
        }
        failure {
            echo 'This will run if the pipeline fails.'
        }
    }
}




