pipeline {
    agent any
    tools { 
        maven 'maven_3.6.1' 
        jdk 'openjdk8' 
    }
    stages {
        stage('---- clean ----') { 
            steps {
                sh "mvn clean"           }
        }
        stage('---- test ----') { 
            steps {
                sh "mvn test"  
            }
        }
        stage('---- package ----') { 
            steps {
                sh "mvn package"
            }
        }
    }
}
