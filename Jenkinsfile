
pipeline {
    agent {
        kubernetes {
            yamlFile 'test.yaml'
            
            defaultContainer 'shell'
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
