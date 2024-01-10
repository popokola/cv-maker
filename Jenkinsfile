pipeline {
    agent any
    triggers {
        cron '* * * * */1'
    }
    options {
        retry(2)
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
            }
        }
        stage('TEST') {
            steps {
                echo 'Building the project...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
            }
        }
    }

    post {
        failure {
            echo 'I failed!'
        }
        success {
            mail to: 'charles258@hotmail.fr',
                 form: "contact@charlesparames.com"
                 subject: 'Pipeline Failure',
                 body: 'The pipeline has failed.'
        }
    }
}