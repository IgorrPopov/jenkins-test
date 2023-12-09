pipeline {
    agent any

    tools {
        nodejs "app" // Use the NodeJS installation defined in Jenkins
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'npm test'
            }
        }

        // stage('Deploy') {
        //     steps {
        //         // Add deployment steps if needed
        //     }
        // }
    }
}
