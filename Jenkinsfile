pipeline{
    agent any
    tools {
            maven 'Maven 3.5.2'
            jdk 'jdk8'
    }

    stages{
        stage('Compile stage'){
            steps{
                bat 'mvn package'
            }
        }
        stage('Testing stage'){
            steps{
                bat 'mvn test'
            }
        }
    }
}
