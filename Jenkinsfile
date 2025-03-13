pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o PES1UG22CS287-1 working.cpp'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './PES1UG22CS287-1'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy stage (Placeholder, modify as needed)'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
