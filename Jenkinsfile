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
            agent {
                label 'slavenode2'
            }
            steps {
                sh 'cd /home/ubuntu/workspace/pipelinejob ; sudo rm -rf test.html'
            }
        }
    }
}
