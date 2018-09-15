@Library('mylibrary') _
pipeline {
    agent any
    tools {nodejs "node"}
    stages {
        stage('Install dependencies') {
            steps {
				echo 'Installing...'
				hello('marvin2')
            }
        }
        stage('Build') {
            steps {
                echo 'Building project...'
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