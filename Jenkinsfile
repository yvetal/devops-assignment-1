pipeline {
    agent {
        label 'local'
    }
    stages {
        stage('Build') {
            steps {
                sh "python3 -m build"
            }
        }
        stage('Archive') {
            steps {
                archiveArtifacts artifacts: 'dist/**/*'
            }
        }
    }
}