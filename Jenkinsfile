pipeline {
    agent any 
    stages {
        stage('Hello') {
            steps {
                echo 'Simon was here!!!1 INSIDE THE JENKINS SCRIPT... Git was a success'
                echo 'Now lets see if sh commands work:'
                sh 'ls'
            }
        }
        stage('Test') {
            steps {
                echo 'Did it fail or WIN!' 
            }
        }
        stage('Build') {
            steps {
                echo 'Docker goes brrrr' 
            }
        }
        stage('Deploy') {
            steps {
                echo 'simonweb.ninja is the place to be?' 
            }
        }
    }
}