
pipeline {
    agent {
        kubernetes {
                    stage('Run shell') {
                        sh 'echo hello world'
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
