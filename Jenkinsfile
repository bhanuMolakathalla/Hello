pipeline {
    agent any
    stages {
    stage('SCM - Checkout') {
    steps {
    git 'https://github.com/bhanuMolakathalla/Hello.git'
    }
    }
        stage('Build') {
            steps {
                def mvnHome = tool name: 'maven-3', type: 'maven'
                
                sh "${mvnHome}/bin/mvn package"
            }
        }
        }
    }
}
