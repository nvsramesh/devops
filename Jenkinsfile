pipeline {
    agent {
        label 'buildserver'
    }
    stages {
        stage('checkout') {
            steps {
                
                
               checkout scm 
            
                
            }
        }
        stage('removing file') {
            steps {
                sh 'cd /home/ubuntu/workspace/pipeline-job ; sudo rm -rf test.html'
            }
        }
    }
}
