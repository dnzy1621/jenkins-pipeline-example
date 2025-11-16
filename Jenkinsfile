pipeline {
    agent any 

    stages {
        stage('Checkout Code') {
            steps {
                echo 'Source code checking out from GitHub.'
            }
        }
        
        stage('Verification Script') {
            steps {
                echo 'Running system verification script...'
                // Command to check the current directory contents
                sh 'ls -l' 
                // Command to display the system's Java version (since Jenkins runs on Java)
                sh 'java -version'
                // This stage now serves as your "Test" equivalent for demonstration
            }
        }
    }
    
    post {
        success {
            echo 'Simple CI Pipeline Finished Successfully!'
        }
        failure {
            echo 'Pipeline Failed! Check Jenkins console output.'
        }
    }
}
