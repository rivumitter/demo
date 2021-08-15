pipeline {
    agent any
    stages {
        stage('compile') {
            steps {
            	withMaven(maven : maven)
                echo 'compiling'
                sh 'mvn clean compile'
            }
        }
	    stage('test') {
           steps {
            	withMaven(maven : maven)
                echo 'compiling'
                sh 'mvn test'
            }
        }
    }
	
}