pipeline{
    agent any

    stages{
        stage('Compile stage'){

            steps{
                withMaven(maven : 'Maven_3_5_2') {
                    bat 'mvn clean compile'
                }
            }
        }
        stage('Testing stage'){
            steps{
                withMaven(maven : 'Maven_3_5_2') {
                    bat 'mvn test'
                }
            }
        }
    }
}
