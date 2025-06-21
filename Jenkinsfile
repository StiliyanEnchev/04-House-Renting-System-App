pipeline {
    agent any

    stages {
        stage('Check out the repository') {
            steps {
                checkout scm
            }
        }

        stage('Install dependencies') {
            steps {
                // Example: Node.js
                bat 'npm install'

                // Other examples:
                // bat 'pip install -r requirements.txt'
                // bat 'mvn install'
                // bat 'gradlew.bat build'
            }
        }

        stage('Run tests') {
            steps {
                // Example: Node.js
                bat 'npm test'

                // Other examples:
                // bat 'pytest'  // for Python
                // bat 'mvn test' // for Java with Maven
                // bat 'gradlew.bat test' // for Gradle
            }
        }
    }
}