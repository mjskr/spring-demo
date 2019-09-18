pipeline {
    agent any
    options {
        ansiColor('xterm')
    }
    stages {

        stage('build') {
            steps {
                sh 'mvn clean package'
            }
            
            tools {
                maven 'default'
            }
        }

    }
}