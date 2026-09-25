pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                bat 'py -m pip install -r requirements.txt'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'py -m pytest'
            }
        }

        stage('Build') {
            steps {
                bat 'py app.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment Successful'
            }
        }
    }
}
