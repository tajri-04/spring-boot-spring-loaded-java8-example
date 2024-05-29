pipeline {
    agent any
    tools {
        maven 'maven363'
    }
    stages {
        stage( 'Get maven version' ){
            steps{
                sh 'mvn --version'
                sh 'mvn package'
                echo 'HELLLLLLLLLLLLLLLO'
            }
        }
        stage( 'sonnar' ){
            steps{
                echo 'SCAN SONNAR'
                sh 'mvn sonar:sonar'
              
            }
        }
    }
}
