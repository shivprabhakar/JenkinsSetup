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
                withMaven(maven : 'maven_4_0_0'){
                    sh 'mvn compile'
                }
            }
        }
    }
}  
