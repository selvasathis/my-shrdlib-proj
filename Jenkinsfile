@Library('my-shared-library') _
pipeline {
    agent any
    stages {
        stage ('scm checkout') {
            steps {
                script {
                    gitCheck()
                }
            }
        }
        // stage ('maven clean') {
        //     steps {
        //         script {
        //             def mvnHome =  tool name: 'maven3', type: 'maven'   
        //             sh "${mvnHome}/bin/mvn clean package"
        //         }
        //     }
        // }
    }
}