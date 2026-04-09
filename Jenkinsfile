pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                sh """
                ssh root@172.16.12.140 '
                    cd /var/www/php-web &&
                    git pull origin main
                '
                """
            }
        }
    }
}