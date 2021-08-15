pipeline {
    agent any
    tools{
    	maven "3.8.2"
    }
    stages {
        stage('compile') {
            steps {
                echo 'compiling the project'
                bat "mvn clean compile"
            }
        }
	    stage('test') {
           steps {
                echo 'compiling'
                bat "mvn test"
            }
        }
    }
    post {
        always {
            cleanWs()
        }
    }
	
}