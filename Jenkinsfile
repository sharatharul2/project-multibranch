//Decalartive Pipeline

pipeline {
    agent any
    stages {
        stage ('Build') {
            steps {
                script{
                     sh 'npm install'
                }
            }
        }
        stage('Docker Build Images') {
            steps {
                script {
                    sh 'docker build -t sharatharul2/multi:v3 .'
                    sh 'docker images'
                }
            }
        }
    }
}
