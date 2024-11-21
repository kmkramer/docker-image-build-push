pipeline {
    agent {
      label docker
    }
    environment {
        CI = 'true'
    }
    stages {
      stage('Deliver for development') {
            when {
                branch 'dev' 
            }
            steps {
                echo "Development"
            }
        }
        stage('Deploy for production') {
            when {
                branch 'main'  
            }
            steps {
                echo "Production"
            }
        }
    }
}
