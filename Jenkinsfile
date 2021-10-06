pipeline {
    agent any
    stages {
        stage('Lint HTML') {
            steps {
                sh 'tidy -q -e index.html'
            }
        }
        stage('Echo hello world') {
            steps {
		    sh 'echo "Hello World with AWS creds"'
            }
        }
    }
}
