pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/KabirGahlowt/WAD.git'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                    echo "Deploying index.html to /var/www/html/"
                    sudo cp index.html /var/www/html/
                '''
            }
        }
    }
}

