pipeline{
        agent { dockerfile true }
		
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
                                sh 'sudo docker build --tag=nuevaimagen:v1'
                        }
                }		

        }
}
