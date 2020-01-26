pipeline{
    agent any
    stages{
        stage('env health check'){
            steps{
                echo 'hello, env health check is done'
            }
        }
        stage('Git checkout'){
            steps{
                git 'https://github.com/shivprabhakar/JenkinsSetup.git'
            }
        }
        stage('compile the test suite'){
            tools{
                maven 'maven_3_6_3'
            }
            steps{
                //def mvnHome = tool name: 'maven_3_6_3', type: 'maven'
                //sh "${mvnHome}/bin/mvn clean compile"
                sh 'mvn clean compile'
            }
        }
    }
}  
