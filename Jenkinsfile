pipeline{
    agent any

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
