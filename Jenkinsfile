pipeline {
    agent any

    stages {
        stage('github') {
            steps {
                checkout scm
            }
        }
        stage('creating a file ') {
            steps {
                sh '''
                    sudo apt install -y apache2
                    sudo ufw allow "Apache"
                    sudo systemctl status apache2
                '''
            }
        }
    }
}
