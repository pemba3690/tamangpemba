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
                echo ' testing website'
            }
        }
        stage('Deploy') { 
            steps {
                echo 'deploying website' 
            }
        }
    }
}
