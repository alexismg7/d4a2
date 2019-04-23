REPOSITORY            TAG                 IMAGE ID            CREATED             SIZE
jenkinsd4a            latest              65982d6e8926        About an hour ago   840MB
edsidocker/d4a        v1                  4dda2dd59ff3        23 hours ago        514MB
php54                 latest              4dda2dd59ff3        23 hours ago        514MB
jenkinsci/blueocean   latest              7959e11c0266        3 days ago          555MB
jenkinsci/jenkins     latest              b589aefe29ff        5 months ago        703MB
php                   5.4-apache          f04f77c9186f        3 years ago         470MB
[backup@ip-192-168-75-21 code]$ vi Jenkinsfile
pipeline{
        agent any
        stages{
                stage('Initial Setup'){
                        steps{
                                sh 'echo Starting..'
                        }

                }
                stage('Checking Docker'){
                        steps{
                                sh 'sudo docker ps'
                        }
                }
                                stage('Build Docker'){
                        steps{
                                sh 'sudo docker build . --tag=nuevaimagen:v1'
                        }
                }

        }
}
~

