pipeline {
    agent any

    stages {
        stage('Git') {
            steps {
               git  'https://github.com/wyzcode-wyz/BoardgameListingWebApp.git'
            }
        }
        
        stage('compile') {
            steps {
                sh 'mvn compile'
            }
        } 
       
         stage('test') {
            steps {
                sh 'mvn clean test'
            }
        } 
       
        stage('package') {
            steps {
                sh 'mvn clean package'
            }
        } 
       
        
    }
    
}
