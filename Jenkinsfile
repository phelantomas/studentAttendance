pipeline{
    agent any

    stages{
        stage('Compile stage'){
            steps{
             bat(/"C:/maven/mvn" -Dmaven.test.failure.ignore clean package/)
            }
        }
        stage('Testing stage'){
            steps{
                bat(/"C:/maven/mvn" -Dmaven.test.failure.ignore test/)
            }
        }
    }
}
