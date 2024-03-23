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
            steps{
                sh 'nohup java -jar target/*.jar &'
            }
        }
    }
}
