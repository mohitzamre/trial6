pipeline {
    agent any

    stages {
        stage('main') {
            when {
                branch 'main'
            }
            steps {
                sh 'echo "hello main"'
            }
        }

        stage('dev') {
            when {
                branch 'dev'
            }
            steps {
                sh 'echo "hello dev"'
            }
        }
    }
}
