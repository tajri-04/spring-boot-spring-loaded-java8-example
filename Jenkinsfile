pipeline {
    agent any
    tools {
        maven 'maven363'
    }
    stages {
        stage( 'sonnar' ){
            steps{
              withSonarQubeEnv('My SonarQube Server') {
                echo 'SCAN SONNAR'
                sh 'mvn clean package sonar:sonar'
              }
           }
        }
    }
}


