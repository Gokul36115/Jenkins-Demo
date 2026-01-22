pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Code checked out from GitHub'
            }
        }

        stage('Build') {
            steps {
                echo 'Listing workspace files'
                sh 'ls -lrt'
            }
        }

        stage('Run Script') {
            steps {
                echo 'Running hello.sh'
                sh 'chmod +x hello.sh'
                sh './hello.sh'
            }
        }
    }
}

