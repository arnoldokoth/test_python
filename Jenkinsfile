pipeline {
    agent any

    environment {
        TEST_VAR = "Some Random Variable"
    }

    stages {
        stage('Install Requirements') {
            steps {
                echo "Installing Requirements..."
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                sh 'nostests -v'
            }
        }
    }
}
