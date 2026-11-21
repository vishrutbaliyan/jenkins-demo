pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building GLA Student Portal...'
                sh 'test -f index.html'
                echo 'Build completed successfully!'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing GLA Student Portal...'
                sh "grep -qi '<html' index.html"
                echo 'All tests passed!'
            }
        }
    }
}
