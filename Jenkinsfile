pipeline {
    agent any
    stages {
        stage('checkout') {
            steps {
                git branch: 'main', credentialsId: '7f56f009-b552-4583-8678-4313f1cbaf40', url: 'git@github.com:ksaohub/vector-role.git'
            }
        }
        stage('molecule run') {
            steps {
           #     sh 'pip3 install molecule molecule-docker'
           #     sh 'molecule init scenario docker --driver-name docker'
                sh 'molecule test -s docker'
            }
        }
    }
}
