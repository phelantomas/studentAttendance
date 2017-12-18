pipeline{
    agent any

    stages{
        stage('Compile stage'){
            steps{
                withMaven(maven : 'Maven'){
                    bat 'mvn clean compile'
                }
            }

        }
        stage('Testing stage'){
            steps{
                withMaven(maven : 'Maven'){
                    bat 'mvn test'
                }
            }
        }
    }
}
