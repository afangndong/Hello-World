pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // This will check out your repository
                checkout scm
            }
        }
        
        stage('Hello World') {
            steps {
                // This assumes you have a script named hello-world.sh in your repository
                sh 'chmod +x hello-world.sh'
                sh './hello-world.sh'
            }
        }
    }
}
