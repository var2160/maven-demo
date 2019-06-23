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
                bat "copy C:\Program Files (x86)\Jenkins\\workspace\deployment using pipeline\gameoflife-web\target\*.war C:\Tools\Apache\webapps
                }
        }
    }
}
