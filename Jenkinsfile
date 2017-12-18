pipeline{
    agent any

    stages{
        stage('Compile stage'){

            steps{
                withMaven(maven : 'Maven_3_5_2') {
                    Sh 'mvn clean compile'
                }
            }
        }
        stage('Testing stage'){
            steps{
                withMaven(maven : 'Maven_3_5_2') {
                    Sh 'mvn test'
                }
            }
        }
    }
}
