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
        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
            }
        }
    }
}