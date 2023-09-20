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
                wget https://download.java.net/java/GA/jdk13.0.1/cec27d702aa74d5a8630c65ae61e4305/9/GPL/openjdk-13.0.1_linux-x64_bin.tar.gz
                tar -xvf openjdk-13.0.1_linux-x64_bin.tar.gz
                mv jdk-13.0.1 /opt/
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
