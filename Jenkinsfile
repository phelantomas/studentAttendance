pipeline {
    agent any
    tools {
        maven 'Maven 3.5.2'
        jdk 'jdk8'
    }
    stages {
        stage ('Initialize') {
            steps {
                bat '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                '''
            }
        }
        stage('Config stage'){
                    steps{
                        bat 'mvn clean compile'
                    }
         }
        stage('Testing stage'){
            steps{
                bat 'mvn test'
            }
        }
    }
}
