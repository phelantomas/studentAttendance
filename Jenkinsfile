pipeline{
    agent any

    stages{
        stage('Compile stage'){
            steps{
                withMaven(maven : 'Maven'){
                    bat 'mvn clean install'
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
