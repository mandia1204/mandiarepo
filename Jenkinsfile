@Library('mylibrary') _
// myTestPipeline(myMessage:'hiiiiii', appName:'security',  runTest: true)

pipeline {
        agent { label 'slave01' }
        tools {nodejs "node"}
        stages {
            stage('copy artifact to ws') {
                steps {
                    copyFiles()
                    sh "pwd"
					sh "ls -l"
                    sh "ls -l dist"
                }
            }
        }
    }