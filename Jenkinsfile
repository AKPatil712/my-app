pipeline {
    agent any
    
    stages {
        stage('clone'){
            steps{
                echo 'cloning'
                bat "mvn clean  my-app"
            }
        }
         stage('build'){
            steps{
                echo 'building'
            }
        }
         stage('test'){
            steps{
                echo 'testing'
                bat "mvn test  my-app"
            }
        }
         stage('deploy'){
            steps{
                echo 'deploying'
                bat "mvn package my-app"
                }
        }
    }
}