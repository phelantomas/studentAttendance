pipeline{
    agent any

    stages{
        stage('Compile stage'){
            steps{
                withMaven(maven : 'Maven'){
                    sh 'mvn clean compile'
                }
            }

        }
        stage('Testing stage'){
            steps{
                withMaven(maven : 'Maven'){
                    sh 'mvn test'
                }
            }
        }
    }
}
