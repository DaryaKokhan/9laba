pipeline {
    agent any
    stages {
        stage('Clean') {
            steps {
                echo 'Cleaning workspace...'
                sh 'ant clean'
            }
        }
        stage('Compile') {
            steps {
                echo 'Compiling source code...'
                sh 'ant compile'
            }
        }
        stage('Package') {
            steps {
                echo 'Packaging application...'
                sh 'ant jar'
            }
        }
        stage('Run') {
            steps {
                echo 'Running application...'
                sh 'ant run'
            }
        }
    }
}
