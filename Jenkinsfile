pipeline {
    agent {
        label 'slavenode'
    }
    stages {
        stage('checkout') {
            steps {
                
                
               checkout scm 
            
                
            }
        }
        stage('removing file') {
            steps {
                node('slavenode2'){
                sh 'cd /home/ubuntu/workspace/pipeline-job ; sudo rm -rf test.html'
                }
            }
        }
    }
}
