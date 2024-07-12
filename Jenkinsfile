pipeline {
    agent { node {label 'AGENT'}}
    stages {
        stage('Build') { 
            steps {
                echo 'building'
            }
        }
        stage('Test') { 
            steps {
                echo 'testing'
            }
        }
        stage('Deploy') { 
            steps {
                echo 'deploying the files'
            }
        }
    }
}
