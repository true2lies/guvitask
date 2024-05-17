pipeline {
    agent any
    stages {
        stage('Welcome') {
            steps {
                echo 'Welcome to the project...'
            }
        }

        stage('Checkout') {
            steps {
                git 'https://github.com/true2lies/guvitask.git'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Skipping build'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Skipping Test'
            }
        }
        stage('Deploy') {
            steps {
                sh 'sudo apt-get update && apt-get install -y nginx'
                sh 'sudo cp index.html /var/www/html/'
                sh 'sudo systemctl restart nginx'
            }
        }
    }

}
