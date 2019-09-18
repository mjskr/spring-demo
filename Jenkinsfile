pipeline {
    agent any
    stages {

        stage('build') {
            options {
                ansiColor('gnome-terminal')
            }
            steps {
                sh 'mvn clean package'
            }
            
            tools {
                maven 'default'
            }
        }

    }
}