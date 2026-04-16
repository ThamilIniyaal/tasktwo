pipeline {
    agent any

    parameters {
        choice(name: 'ENVIRONMENT', choices: ['dev', 'test'], description: 'Select environment')
    }

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/your-username/your-repo.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building in ${params.ENVIRONMENT} environment..."
            }
        }

        stage('Test') {
            steps {
                echo "Testing in ${params.ENVIRONMENT} environment..."
            }
        }
    }
}
