pipeline {
    agent any 
    stages {
        stage('Building WAR file') { 
            steps {
                bat "mvn clean install"
                echo "*************Build Created***************"
            }
        }
        stage('Deploy') { 
            steps {
                 echo "deployment started"
                 bat 'xcopy "C:\\Program Files (x86)\\Jenkins\\workspace\\MVN pipeline deploy from SCM\\gameoflife-web\\target\\gameoflife.war" "C:\\Tools\\Apache\\webapps"'
                 echo "**************Deployment Completed****************"
            }
        }
    }
}
