pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/RiteshMurari/SL-MAVEN-8-FEB-BACTH'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package' // Use 'sh' instead of 'bat' for Linux-based Jenkins
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test' // Use 'sh' for Linux
            }
        }
    }
}
