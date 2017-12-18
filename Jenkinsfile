pipeline{
    agent any

    stages{
        stage('Compile stage'){
            steps{
                withMaven(maven : 'maven'){
                    bat 'mvn clean install'
                }
            }
        }
        stage('Testing stage'){
            steps{
                withMaven(maven : 'maven'){
                    bat 'mvn test'
                }
            }
        }
    }
}
