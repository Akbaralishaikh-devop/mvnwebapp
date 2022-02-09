pipeline {
    agent any
    tools
    {
        maven 'MAVEN'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Hello World'
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'e7767c5c-0f0e-421a-8782-66384b0bfad6', url: 'https://github.com/Khalid12Clover/mvnwebapp.git']]])
                bat "mvn -Dmaven.test.failure.ignore=true clean package"
            }
        }
    }
    post{
        always{
            junit(
                allowEmptyResults:true,
                testResults: '**/test-results/*.xml'
                )
        }
    }
}
