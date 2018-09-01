pipeline {
    agent any
    tools {nodejs "node"}
    stages {
        stage('Install dependencies') {
            steps {
				echo 'Installing...'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
    }
	post {
		always {
			archiveArtifacts 'dist/**/*'
		}
	}
}