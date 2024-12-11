pipeline {
    agent any
    
    stages{
        stage('myweb') {
            steps {
                sh 'sudo rm -rf /var/www/html/*'
                sh 'sudo rm -rf /var/www/html/.git'
                sh 'sudo yum install httpd -y'
                sh 'sudo systemctl start httpd'
                sh 'sudo systemctl enable httpd'
                sh 'sudo git clone https://github.com/ashwindevop/myweb1may.git  /var/www/html'
            }
        }
    }
}
