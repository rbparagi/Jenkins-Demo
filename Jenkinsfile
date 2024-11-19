pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M398" and add it to the path.
        maven "M398"
    }

    stages {
        stage('Configure Git Safe Directory') {
            steps {
                // Mark the Jenkins workspace as a safe directory for Git
                sh 'git config --global --add safe.directory "$WORKSPACE"'
            }
        }

        stage('Echo Version') {
            steps {
                sh 'echo Print Maven version'
                sh 'mvn -version'
            }
        }
    }
}
