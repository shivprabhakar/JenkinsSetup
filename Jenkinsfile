pipeline{
    agent any
    stages{
        stage('env health check'){
            steps{
                echo 'hello, env health check is done'
            }
        }
        stage('compile the test suite'){
            steps{
                mvn clean compile
            }
        }
    }
}