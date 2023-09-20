pipeline {
    agent {
       label "build-server"
    }
    stages {
        stage('Build') {
            steps {
                git clone 'https://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@github.com/rahulmula/tweet-trend.git'
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
