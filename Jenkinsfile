pipeline {
    agent any
    tools {
        maven 'maven363'
    }
    stages {
        stage( 'sonnar' ){
            steps{
              withSonarQubeEnv('sonar-6') {
                echo 'SCAN SONNAR'
                sh 'mvn clean package sonar:sonar'
              }
           }
        }
    }
}


