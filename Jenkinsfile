pipeline {
    agent any
    
    stages {

        stage('clone') {
            steps{
                echo 'cloning'
                bat "mvn clean "
            }
        }
         stage('test') {
            steps{
                echo 'testing'
                bat "mvn test"
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