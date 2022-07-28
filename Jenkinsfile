pipeline {
    agent any 
    stages {
        stage('removing old files') { 
            steps {

                sh "sudo rm -rvf /var/www/html/*"
                sh "sudo rm -rvf /var/www/html/.git"
                sh " sudo rm -rvf /var/www/html/.ht* "
              
                
            }
        }
        stage('Cloning repo') { 
            steps {
                sh " sudo git clone https://github.com/pemba3690/tamangpemba.git  /var/www/html/"
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
