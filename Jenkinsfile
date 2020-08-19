
pipeline {
    agent any

    stages {
        
        stage('deploy hello minikube') {
            steps {
                sh 'kubectl create -f deployment.yaml'
            }
        }
        stage('test deployment') {
            steps {
                sh 'kubectl get pods'
            }
        }
        stage('Sleeping For Exactly 1 minute') {
            steps {
                sleep time: 1, unit: 'MINUTES'
            }
        }
        
        stage('cleanup') {
            steps {
                sh 'kubectl delete service hello-node'
                sh 'kubectl delete deployment hello-node'
            }
        }
    }
}
