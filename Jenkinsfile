pipeline {
    agent any
    stages {
        stage('clone repo and clean') { 
            steps {
                sh "git clone https://github.com/vitsindelar/mvn_quick_start.git"
                sh "mvn clean"
                            }
        }
        stage('Test') { 
            steps {
                sh "mvn test"  
            }
        }
        stage('Deploy') { 
            steps {
                sh "mvn package"
            }
        }
    }
}
