@Library('my-shared-library') _
pipeline {
    agent any
    stages {
        stage ('scm checkout') {
            steps {
                script {
                    gitCheck(
                        branch: "main",
                        url: "https://github.com/selvasathis/my-shrdlib-proj.git"
                    )                    
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