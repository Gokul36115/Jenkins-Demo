pipeline {
    agent any

    stages {
        stage('Run Script') {
            steps {
                echo 'Running hello.sh'
                sh './hello.sh'
                sh 'exit 1'
            }
        }
    }
}

