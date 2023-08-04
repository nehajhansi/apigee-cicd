#!groovy

pipeline {
    agent any
    tools {
        maven 'M2'
        jdk 'JDK'
        nodejs 'NODEJS'
    }

    stages {
        stage('Deploy to Production') {
            steps {
                 //deploy using maven plugin
                 
                 // deploy only proxy and deploy both proxy and config based on edge.js update
                //bat "sh && sh deploy.sh"
                bat "mvn -f HR-API/pom.xml install -Pprod -Dusername=${apigeeUsername} -Dpassword=${apigeePassword} -Dapigee.config.options=update"
            }
        }
    }
}
