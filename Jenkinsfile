pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
               git branch: 'main', url: 'https://github.com/sgayatrijadhav-hub/my-gradle-app.git'
            }
        }

        stage('Build') {
            steps {
                sh 'gradle build'
            }
        }

        stage('Run') {
            steps {
                sh 'gradle run'
            }
        }
    }
}
