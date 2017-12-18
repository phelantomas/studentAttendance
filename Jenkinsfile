pipeline{
    agent any

    stages{
        stage('Compile stage'){
            steps{
                withMaven(maven : 'Maven 3.5.2'){
                    bat 'mvn package'
                }
            }
        }
        stage('Testing stage'){
            steps{
                withMaven(maven : 'Maven 3.5.2'){
                    bat 'mvn test'
                }
            }
        }
    }
}
