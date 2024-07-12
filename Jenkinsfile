pipeline {
    agent { 
        node { 
            label 'Agent' 
        } 
    }
    stages {
        stage('Build') { 
            steps {
                echo 'building'
                sh '''
                    ls -ltr
                    pwd
                    echo "hello script"
                '''
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
    post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if the pipeline succeeds'
        }
        failure {
            echo 'This will run only if the pipeline fails'
        }
    }
}
