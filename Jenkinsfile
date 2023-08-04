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
                bat "mvn -f HR-API/pom.xml install -Ptest-env -Dbearer=ya29.a0AfB_byAobwyhrlKckttEmqtUxk7pM95GX7z-nnC1UN2zGdPHULGhbVYq_bnCnJtAwKPYry1iQdviPNMO-2PPqVKwpzQeEHxRq0E5S9u2k2Wp8Cl7KkMko044ja3yPmdJcXm3FcL03eMOxCah4RC05bu6zokjxpaenvJTK-d5rjEyc2Hz2isYlXRnZ7Vtak3h3kbvsUFwJZQhpICbd6nfWvkdM8M06VYN24s0X1yhOn4JW7a8QDowr5cmMdcs-_u9A3LIUkuvlUgLVsCT0L8s4hL1y8ZkvNjxA00H1Ul3EnWeVUMP8YqtfZrPKwdD9STBQRKM3KqygpWpY0PxK2CK4_fj9tsam1F3mwwcsJIJMkZtioPspaHOfLtXDiiBeSC_0aZKZTROoxB0nwT07EBCbhg8aCgYKAe8SARMSFQHsvYlskNRH534Yhhq8Nzb8spDQUQ0415 -Dapigee.config.options=update"
            }
        }
    }
}
