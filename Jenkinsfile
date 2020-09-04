pipeline {
    agent any 
    stages {
        stage('clean') { 
            steps {
                bat "mvn clean -f JavaJenkins"
            }
        }
        stage('Test') { 
            steps {
                bat "mvn test -f JavaJenkins"
            }
        }
        stage('Deploy') { 
            steps {
                bat "mvn package -f JavaJenkins"
            }
        }
    }
}
