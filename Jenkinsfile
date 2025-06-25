pipeline {
    agent any

    stages {
        stage('github') {
            steps {
                checkout scm
            }
        }
        stage('installing a apache') {
            steps {
                sh '''
                    sudo apt install -y apache2
                    sudo ufw allow "Apache"
                    sudo systemctl status apache2
                '''
            }
        }
	stage ('creating a file')
	    steps{
		sh 'ls -l'
    }
}
