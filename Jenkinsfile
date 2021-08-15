pipeline {
    agent any
    stages {
        stage('compile') {
            steps {
            	withMaven(maven : maven)
                echo 'compiling the project'
                bat "mvn clean compile"
            }
        }
	    stage('test') {
           steps {
            	withMaven(maven : maven)
                echo 'compiling'
                bat "mvn test"
            }
        }
    }
	
}