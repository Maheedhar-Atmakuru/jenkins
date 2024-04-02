pipeline{
    agent any 
    environment {
        ENV_URL = "pipeline.google.com"
    }
    stages {
        stage{"First Stage"} {
            steps {
                sh "echo Welcome World!"
                sh "echo ${ENV_URL}"
            }
        }
        stage{"Second Stage"} {
            environment {
                ENV_URL = "stage.google.com"
            }
            steps {
                sh "echo Welcome World!"
                sh "echo ${ENV_URL}"
            }
        }
        stage{"Third Stage"} {
            steps {
                sh "echo Welcome World!"
            }
        }
    }
}