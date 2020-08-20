
pipeline {
    agent {
        kubernetes {
            label 'minikube'
          
            
            yamlFile 'test.yaml'
        }
    }
    stages {
        stage('Main') {
            steps {
                sh 'hostname'
            }
        }
    }
}
