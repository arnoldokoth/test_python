pipeline {
    agent any
    environment {
        TEST_VAR = "Some Random Variable"
    }

    stage('Install Requirements') {
        sh 'pip install -r requirements.txt'
        sh 'nostests -v'
    }
}
