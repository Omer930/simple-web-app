pipeline {
    agent any

    stages {
        
        stage('Building') {
            steps {
                nodejs('NodeJS'){
                    sh 'npm install'
                    sh' npm build'
            }
        }
        stage('Artifact Archiving') {
            steps {
                echo 'The Artifact will be uploaded to an artifact repository'
            }
        }
        stage('Testing') {
            steps {
                echo 'The Artifact will be tested'
            }
        }
        stage('Staging') {
            steps {
                echo 'The Artifact is staged onto the staging server'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'The software will now be deployed!'
            }
        }
    }    
}
