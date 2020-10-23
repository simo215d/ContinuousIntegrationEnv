pipeline {
    agent any 
    stages {
        stage('Hello') {
            steps {
                echo 'Simon was here!!!1 INSIDE THE JENKINS SCRIPT... Git was a success'
                echo 'Now lets see if sh commands work:'
                sh 'ls'
                echo 'Ultimate test do an npm command for libs omg:'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Did it fail or WIN!'
                sh 'npm run test' 
            }
        }
        stage('Build') {
            steps {
                echo 'Docker goes brrrr'
                sh 'docker-compose up' 
            }
        }
        stage('Deploy') {
            steps {
                echo 'simonweb.ninja is the place to be?' 
            }
        }
    }
}