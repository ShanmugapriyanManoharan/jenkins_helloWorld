pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Using triple quotes and Windows-style path with double backslashes
                   powershell '''
                    & "C:\\Python312\\python.exe" "hello.py"
                '''
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                powershell 'Write-Output "Running Windows tests..."'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                powershell 'Write-Output "Deploying on Windows..."'
            }
        }
    }
}
