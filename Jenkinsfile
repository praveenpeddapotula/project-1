pipeline {
    agent any 
    tools {
        java 'JDK17'
        maven 'MAVEN3.9.9'
    }
    stages {
        stage ('checkout') {
            steps {
                script {
                    git branch 'main';
                }
            }
        }
    }
}