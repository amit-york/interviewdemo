pipeline {
    agent any
    environment {
        building = 'Building the project'
        testing = 'Testing the project'

    }
    stages {
        stage('Build'){
            steps {
                echo "${building}"
            }
        }
        stage('Test'){
            steps {
                echo "${testing}"
            }   
        }
        stage('Get Git Tag') {
            steps {
                script {
                    sh "git fetch --tags"
                    VERSION = sh(script: "git describe --tags --abbrev=0", returnStdout: true).trim()
                    echo "Release Version: ${VERSION}"
                }
            }
        }
    }
}



// This Jenkinsfile defines a simple CI/CD pipeline with two stages: Build and Test.