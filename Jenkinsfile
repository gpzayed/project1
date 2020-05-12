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
                sh 'echo "Today is $(date) and this machine name is: $(hostname)."'
                sh 'echo "Thanks."'
            }
        }
        stage('SecondStage') {
            steps {
                sh 'Well done, project moved to second stage.'
                sh 'Some info about system: $(uname -a)'
            }
        }
        stage('Final') {
            steps {
                sh 'Well done, project completed on $(date)'
            }
        }
    }
}
