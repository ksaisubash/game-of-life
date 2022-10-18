pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                sh 'echo hello'
            }
        }
        stage('learning') {
            agent { label 'ubuntu_node-1' }
            steps {
                git url: 'https://github.com/ksaisubash/game-of-life.git',
                    branch: 'master'
            }
        }
    }
}
