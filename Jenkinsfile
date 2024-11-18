pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M398" and add it to the path.
        maven "M398"
    }

    stages {
        stage('Echo Version') {
            steps {
                sh 'echo Print Maven version'
                sh 'mvn -version'
            }
        }
    }
}
