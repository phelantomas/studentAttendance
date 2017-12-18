pipeline{
    agent any

    stages{
        stage('Compile stage'){
            steps{
                bat 'mvn clean install'
            }
        }
        stage('Testing stage'){
            steps{
                    bat 'mvn test'
            }
        }
    }
}
