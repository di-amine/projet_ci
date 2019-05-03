pipeline {
    agent any
    tools {
        maven 'maven3'
    }
    stages {
        stage ('Checkout') {
            steps {
                git url: 'https://github.com/di-amine/projet_ci.git', credentialsId: '70ecb8f7-b239-431a-af07-c9049a10d012', branch: 'dev'
            }
        }
        stage ('Build') {
   
            steps {
                echo 'Build'
                sh 'mvn install'
            }
        }
        stage ('Deploy') {
            
            steps {
                echo 'Deploy'
            }

        }
    }
}
