pipeline {
    agent any
    environment {
        building = 'Building the project'
        testing = 'Testing the project'

    }
    stages {
        stage('Build'){
            steps {
                echo ${building}
            }
        }
        stage('Test'){
            steps {
                echo ${testing}
            }   
        }
    }
}


// This Jenkinsfile defines a simple CI/CD pipeline with two stages: Build and Test.