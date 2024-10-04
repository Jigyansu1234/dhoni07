pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clone the repository
                git url: 'https://github.com/yourusername/your-repo.git', branch: 'main'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Install Node.js and npm dependencies
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                // Run tests (for simplicity, we'll assume there are no tests here)
                echo 'Running Tests...'
                // Normally you'd use something like: `sh 'npm test'`
            }
        }

        stage('Build') {
            steps {
                // Build the project (for a simple Node.js app, this could be optional)
                echo 'Building...'
            }
        }

        stage('Deploy') {
            steps {
                // Start the application (could be PM2, Docker, etc.)
                echo 'Deploying...'
                sh 'npm start'
            }
        }
    }
}
