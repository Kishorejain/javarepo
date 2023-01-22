pipeline {
    agent any
    stages {
        stage('git') {
            steps {
                 echo "this is git stage to clone the repository"
                 git 'https://github.com/Kishorejain/javarepo.git'
                         }
        }
            stage('mavenbuild') {
            steps {
                echo "this is build stage"
                sh 'mvn clean install'
            }
        }
		stage('Deploy') {
            steps {
                echo "this is build deploy"
            }
        }
		stage('test') {
            steps {
                echo "this is build test"
            }
        }
    }
}
