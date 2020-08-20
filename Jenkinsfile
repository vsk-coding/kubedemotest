
pipeline {
    agent {
        kubernetes {
            stages{
                    stage('Run shell') {
                        sh 'echo hello world'
                    }  
            }
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
