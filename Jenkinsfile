

pipeline {
    agent {docker {image 'maven:3.6.3'}}
    stages {
        stage('Build'){
            steps {
                sh 'sudo maven --version'
                echo "Build"
            }
        }
        stage('Test'){
            steps{
                echo"Hello world! Swathi"
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
