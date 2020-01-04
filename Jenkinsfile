pipeline {
    agent any
    
    stages {

        stage('clone') {
            steps{
                echo 'cloning'
                bat "mvn clean "
            }
        }
        stage('deploy') {
            steps{
                echo 'deploying'
                bat "mvn package"
                }
        }
    }
}