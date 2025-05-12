pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/SrikarVanaparthy/Jenkins-usecase1.git'
            }
        }

        stage('Run Python Script') {
            steps {
                echo 'Running users1.py...'
                bat 'python3 users1.py'
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution finished.'
        }
    }
}
