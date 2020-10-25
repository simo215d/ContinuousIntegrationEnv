pipeline {
    agent any 
    stages {
        stage('Hello') {
            steps {
                echo 'JENKINS SCRIPT... Git was a success'
                echo 'Now lets see if sh commands work:'
                sh 'ls'
                echo 'npm command for libs:'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'fail? win!'
                sh 'npm run test' 
            }
        }
        stage('Build') {
            steps {
                echo 'Docker goes brrrr'
                sh 'docker-compose up -d' 
            }
        }
        stage('Deploy') {
            steps {
                echo 'simonweb.ninja is the place to be'
                sh 'az webapp up --name simonweb' 
            }
        }
    }
}