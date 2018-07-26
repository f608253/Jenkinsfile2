pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh '''
                uname -a
                ls -lrt
                ping -c50 google.co.in
                cd $HOME && pwd && cd /home/ec2-user/scripts $$ sudo find / -size +1k -print
                '''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
