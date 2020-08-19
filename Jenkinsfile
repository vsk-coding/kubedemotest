
pipeline {
    agent {
        kubernetes {
            label 'jenkinspods'
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
