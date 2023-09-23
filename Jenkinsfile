pipeline{
    agent any
    stages{
        stage('checkout'){
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'e892360d-e476-4beb-9b38-d8ac246f70ff', url: 'https://github.com/tiwariansuman/jenkins_testing.git']])
            }
        }
        stage('complie'){
            steps{
                bat '''gcc sample2.c -o sample
sample'''
            }
        }
    }
}
