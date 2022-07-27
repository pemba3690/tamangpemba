pipeline {
    agent any 
    stages {
        stage('website running') { 
            steps {
                sh ' echo building website'
            }
        }
        stage('Test') { 
            steps {
                sh ' echo testing website'
            }
        }
        stage('Deploy') { 
            steps {
                sh 'deploying website' 
            }
        }
    }
}
