pipeline {
    agent any
    triggers {
        cron '* * * * */1'
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
        success {
            mail to: 'charles258@hotmail.com',
                 subject: 'Pipeline Success',
                 body: 'The pipeline has been succefully deployed.'
        }
    }
}