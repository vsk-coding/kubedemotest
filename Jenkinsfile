
pipeline {
    agent {
        kubernetes {
            label 'jenkins-slave'
          
            
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
