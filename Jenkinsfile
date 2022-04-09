pipeline {
    agent any 
    stages {
        stage('clone repo and clean') { 
            steps {
                //sh "rm -rf devops"
                //sh "git clone https://github.com/PavanVaduguru/devops.git"
                sh "mvn clean"
            }
        }
        stage('Test') { 
            steps {
                //sh "rm -rf devops"
                sh "mvn test" 
            }
        }
        stage('Deploy') { 
            steps {
                //sh "rm -rf"
                sh "mvn package"
            }
        }
    }
}
