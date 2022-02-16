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
                sh 'cd /home/ubuntu/workspace/pipelinejob ; sudo rm -rf test.html'
                }
            }
        }
    }
}
