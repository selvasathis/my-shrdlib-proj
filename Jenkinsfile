pipeline {
    agent any
    stages {
        stage ('scm checkout') {
            steps {
                script {
                    git branch: 'main', url: 'https://github.com/selvasathis/my-app-master.git'  
                }
            }
        }
        stage ('maven clean') {
            steps {
                script {
                    def mvnHome =  tool name: 'maven3', type: 'maven'   
                    sh "${mvnHome}/bin/mvn clean package"
                }
            }
        }
    }
}