pipeline {
    agent any

    stages {
        stage('github') {
            steps {
                checkout SCM
            }
        }
        stage('creating a file ') {
            steps {
                sh '''
                    sudo apt install apache2
                    sudo ufw allow "Apache"
                    sudo systemctl status apache2
                '''
            }
        }
    }
}
