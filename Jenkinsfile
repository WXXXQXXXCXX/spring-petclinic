pipeline {
    agent any
    tools { 
        maven 'maven 3.3.1' 
        jdk 'jdk17' 
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
