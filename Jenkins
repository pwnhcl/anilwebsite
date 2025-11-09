pipeline {
    agent any

    stages {
        stage('Prepare') {
            steps {
                echo 'Code checked out by Jenkins from SCM.'
                // List files to verify checkout
                sh 'ls -l'
            }
        }

        stage('Build/Deploy') {
            steps {
                echo 'Add your build or deployment commands here.'
                // Example:
                // sh './deploy.sh'    // or any build commands you need
            }
        }
    }

    post {
        success {
            echo '✅ Pipeline executed successfully!'
        }
        failure {
            echo '❌ Pipeline failed.'
        }
    }
}
