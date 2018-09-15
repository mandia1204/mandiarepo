@Library('mylibrary') _
import restaurant.sample.Person
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
                echo 'Building...'
                script {
					def p = new Person()
					def r = p.hello()
					println(r)
				}
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