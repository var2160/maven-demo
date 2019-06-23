pipeline {
    agent any 
    stages {
        stage('Clean') { 
            steps {
                bat "mvn clean"
            }
        }
        stage('Creating War File') { 
            steps {
                bat "mvn install"
            }
        }
        stage('Deploy') { 
            steps {
                echo "War file deployed successfully"
            }
        }
    }
}
