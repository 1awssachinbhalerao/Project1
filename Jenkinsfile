pipeline {
    agent {
        node{
            label 'maven'
        }
    }
    environment {
        PATH = "/opt/apache-maven-3.9.6:$PATH"
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean verify'
            }
        }
    }
}
