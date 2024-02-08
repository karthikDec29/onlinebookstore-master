pipeline {
    agent any
    tools
    maven 'maven'
}
    stages {
        stage('Clone the repository') {
            steps {
                git 'https://github.com/karthikDec29/onlinebookstore-master.git'
            }
        }
        stage('Build the code') {
            steps {
             sh 'mvn clean install'
            }
        }
        stage('docker image') {
            steps {
             sh 'docker build -t ashok .'
                
            }
        }
    }
}
