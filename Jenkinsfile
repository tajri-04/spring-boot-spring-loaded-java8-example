pipeline {
    agent any
    tools {
        maven 'maven363'
    }
    stages {
        stage( 'sonnar' ){
            steps{
              withSonarQubeEnv('Sonar') {
                echo 'SCAN SONNAR'
                sh 'mvn clean package sonar:sonar'
              }
           }
        }
    }
}


