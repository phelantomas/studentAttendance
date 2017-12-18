pipeline{
    agent any
    stage('Compile stage'){
        steps{
            bat 'mvn clean compile'
        }
    }
    stage('Testing stage'){
        steps{
            bat 'mvn test'
        }
    }
}
