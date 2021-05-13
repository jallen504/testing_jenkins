pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build Stage:'
                chmod +x gradlew
                withGradle{
                    gradlew build
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Test Stage'
            }
        }
    }
}