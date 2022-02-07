pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo "Build Done"
                mvn package
            }
        }
        stage('Test') { 
            steps {
                echo "Test Done"
            }
        }
        stage('Deploy') { 
            steps {
                echo "Deployment Done"
            }
        }
    }
}
