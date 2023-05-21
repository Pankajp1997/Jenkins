pipeline {
    agent any 
    stages {
        stage ('checkout') {
            step {
                git branch: 'master', url: 'https://github.com/prasadcloud/maven2.git'
            }
        }
    }
    stages {
        stage ('Build') {
            step {
                sh 'mvn clean install'
            }
        }
    }
    stages {
        stage ('Test') {
            step {
                sh 'mvn test'
            }
        }
    }

}
