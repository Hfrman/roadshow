pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh './gradlew clean' 
            }
        }
        stage('Test'){
            steps {
                 sh './gradlew check'  
            }
        }
        stage('Greet') {
            steps {
                echo 'hello world!'
            }
        }
    }
}
