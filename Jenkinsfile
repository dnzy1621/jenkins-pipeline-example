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
                echo 'Running system verification script (Windows)...'
                // CHANGE: Use 'bat' for Windows Command Prompt execution
                bat 'dir' // Windows equivalent of 'ls -l'
                
                // CHANGE: Use 'bat' for Windows Command Prompt execution
                bat 'java -version' 
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
