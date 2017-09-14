pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps { 
                sh 'mvn clean install' 
            }
        }
        stage('Test'){
            steps {
                sh 'make check'
                junit '**/target/surefire-reports/*.xml' 
            }
        }
        stage('Deploy') {
            steps {
                sh 'make publish'
            }
        }
    }
}
