pipeline {
    agent {
       label "build-server"
    }
    stages {
        stage('Build') {
            steps {
                //git branch: 'main', credentialsId: 'Github_cred', url: 'https://github.com/rahulmula/tweet-trend.git'
                sh '''
                pwd
                git fetch https://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@github.com/rahulmula/tweet-trend.git
                pwd
                cd tweet-trend
                mvn compile
                '''
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
