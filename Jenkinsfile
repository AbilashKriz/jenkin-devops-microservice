pipeline {
    agent any

    environment {

        dockerHome = tool 'MyDock'
        mavenHome = tool 'MyMaven'
        PATH = '$dockerHome/bin:$mavenHome/bin:$PATH'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
                sh 'docker --version'
            }
        }
    }
}
