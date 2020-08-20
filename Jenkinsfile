
pipeline {
    agent {
        kubernetes {
                node(POD_LABEL) {
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
