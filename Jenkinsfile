pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
        stage('Run Python Script') {
            steps {
                script {
                    if (isUnix()) {
                        sh 'python3 app.py'
                    } else {
                        bat 'python app.py'
                    }
                }
            }
        }
    }
}
