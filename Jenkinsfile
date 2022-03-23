pipeline {
    environment {
        JENKINS_USER_NAME = "${sh(script:'id -un', returnStdout: true).trim()}"
        JENKINS_USER_ID = "${sh(script:'id -u', returnStdout: true).trim()}"
        JENKINS_GROUP_ID = "${sh(script:'id -g', returnStdout: true).trim()}"
    }
    agent any
    stages {
        stage('Build'){
            steps {
                echo "Build"
                echo "$PATH"
                echo "BUILD_NUMBER - $env.BUILD_NUMBER"
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
