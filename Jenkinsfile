pipeline {
    agent any

    triggers {
        pollSCM('H/2 * * * *')
    }

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building Application'
                sh 'echo Build Successful'
            }
        }

        stage('Test') {
            steps {
                echo 'Running Tests'
                sh 'echo Tests Passed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying Application'
                sh 'echo Deployment Successful'
            }
        }
    }
}
