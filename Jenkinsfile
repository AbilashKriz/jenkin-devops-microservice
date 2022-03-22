pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo"Hello world ! Abilash"
            }
        }
        stage('Test') {
            steps{
                echo"Hello world! Swathi"
            }            
        }
        stage('example' {
            steps {
                echo"Example world"
            }
        }
    } 
    post {
        always {
            echo "I run always"
        }
        success {
            echo "I run when it's successful"
        }
        failure {
            echo "I run when failed"
        }
    }
}
