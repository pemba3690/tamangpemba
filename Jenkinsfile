pipeline {
    agent any 
    stages {
        stage('installing httpd') { 
            steps {

                sh "sudo rm -rvf /var/www/html/*"
                sh "sudo rm -rvf /var/www/html/.git"
                
            }
        }
        stage('Cloning repo') { 
            steps {
                sh "sudo git clone git@github.com:pemba3690/tamangpemba.git /var/www/html/"
                // 
            }
        }
        stage('Reloading code') { 
            steps {
                sh "sudo systemctl reload httpd"
            }
        }
    }
}
