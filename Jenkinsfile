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
        stage('create pull request'){
            when {branch 'dev'}
            steps{
                sh 'gh create --B main --H dev --title "PR"  --body "auto pr"'
            }
        }
        
        
    }
}
