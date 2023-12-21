pipeline {
    // agent { label "docker" }
    stages {
        stage('Clone Repo') {
            steps {
                checkout scm
            }
        }
        stage('Docker Build') {
            steps {
                sh "docker build -t web:1.0 ."
            }
        }
    }
}