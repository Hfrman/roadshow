pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh './gradlew jenkinstest' 
            }
        }
        stage('Test'){
            steps {
                junit 'reports/**/*.xml' 
            }
        }
        stage('Greet') {
            steps {
                echo 'hello world!'
            }
        }
    }
}
