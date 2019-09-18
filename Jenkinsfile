pipeline {
    agent any
    options {
        ansiColor('xterm')
    }
    stages {

        stage('get repo') {
          steps {
            git poll: false, url: 'https://github.com/neaho/spring-demo'
          }
        }
        
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