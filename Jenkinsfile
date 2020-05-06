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
                sh 'echo "Hello World, again"'
                sh 'Today is $(date) and this machine name is: $(hostname).'
            }
        }
    }
}
