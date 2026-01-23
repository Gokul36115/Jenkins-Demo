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

    post {
        success {
            echo 'Pipeline succeeded'
        }
        failure {
            echo 'Pipeline failed – investigate logs'
        }
        always {
            echo 'Pipeline finished (success or failure)'
        }
    }
}

