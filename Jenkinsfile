pipeline {
    agent any
    tools { 
        maven 'maven' 
    }
    stages {
        stage('Build') { 
            steps {
                sh './mvnw package' 
            }
        }
        stage('Run') {
            sh 'java -jar target/*.jar'
        }
    }
}
