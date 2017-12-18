pipeline{
    agent any

    stages{
        stage('Compile stage'){
            steps{
             bat(/"${mvnHome}\bin\mvn" -Dmaven.test.failure.ignore clean package/)
            }
        }
        stage('Testing stage'){
            steps{
                bat(/"${mvnHome}\bin\mvn" -Dmaven.test.failure.ignore test/)
            }
        }
    }
}
