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
                bat '"C:\\Users\\Admin-BL\\AppData\\Local\\Programs\\Python\\Python314\\python.exe" users1.py'

               
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution finished.'
        }
    }
}
