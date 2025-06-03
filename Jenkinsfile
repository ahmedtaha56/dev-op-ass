pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                echo 'Cloning the repository...'
                // If using Git, Jenkins will clone it automatically.
                // Otherwise, you can use `git` manually here.
            }
        }

        stage('Build') {
            steps {
                echo 'Checking HTML file...'
                sh 'ls -l *.html'
            }
        }

        stage('Serve (Optional)') {
            steps {
                echo 'You can serve HTML using Python if needed.'
                // Uncomment below to serve the HTML on localhost:8000
                // sh 'nohup python3 -m http.server 8000 &'
            }
        }
    }

    post {
        success {
            echo 'Build finished successfully!'
        }
        failure {
            echo 'Something went wrong!'
        }
    }
}
