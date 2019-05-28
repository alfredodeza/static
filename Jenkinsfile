pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
        stage('Run in AWS') {
            steps {
                withAWS(credentials:'aws-static') {
		    sh 'echo "Hello World with AWS creds"'
                }
            }
        }
    }
}
