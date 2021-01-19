pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World2'
            }
        }
		stage('Git') {
            steps {
                git "https://github.com/shyampandu/javaproject.git"
            }
        }
		stage('CLean') {
            steps {
                sh "mvn clean "
            }
        }
		stage('Code Testing') {
            steps {
                sh "mvn test"
            }
        }
		stage('package') {
            steps {
                 sh "mvn package"
            }
        }
		stage('compile') {
            steps {
                 sh "mvn compile"
            }
        }
		
    }
}
