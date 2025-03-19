pipeline {
    agent any 
    tools {
        jdk 'JDK17'
        maven 'MAVEN3.9.9'
    }
    stages {
        stage ('checkout') {
            steps {
                script {
                    git url:'https://github.com/praveenpeddapotula/project-1.git' , branch: 'main'
                }
            }
        }
        stage ('build') {
            steps {
                sh 'mvn clean build'
            }
        }
        stage ('test') {
            steps {
                sh 'mvn test'
            }
        }
        stage ('package') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}