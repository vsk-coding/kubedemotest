
pipeline {
    agent {
        kubernetes {
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
