pipeline {
    agent any

    tools {
        // Use the NodeJS installation configured in Jenkins
        nodejs 'NodeJS'
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout your project repository
                git url: 'https://github.com/your_username/your_playwright_project.git'
            }
        }

        stage('Install dependencies') {
            steps {
                // Install dependencies using npm
                sh 'npm install'
            }
        }

        stage('Run tests') {
            steps {
                // Run your Playwright tests
                sh 'npx playwright test'
            }
        }
    }
}