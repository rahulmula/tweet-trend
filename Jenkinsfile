pipeline {
    agent {
       label "build-server"
    }
    stages {
        stage('Build') {
            steps {
                git 'https://github.com/rahulmula/tweet-trend.git'
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
