pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo "Build Done"
                javac HelloWorld.java
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
