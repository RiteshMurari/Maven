pipeline { 
    agent any 
    stages { 
        stage('Checkout') { 
            steps { 
                git 'https://github.com/your/repository.git'  
            } 
        } 
        stage('Build') { 
            steps { 
                sh 'mvn clean package' 
            } 
        } 
        stage('Test') { 
            steps { 
                sh 'mvn test' 
            } 
        } 
        stage('Deploy') { 
            steps { 
                echo 'Deploying...'
            } 
        } 
    }  
    post { 
        success { 
            echo 'Pipeline executed successfully!' 
        } 
        failure { 
            echo 'Pipeline failed!' 
        } 
    } 
}
