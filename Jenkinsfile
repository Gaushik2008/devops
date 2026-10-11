
pipeline {
    agent any

    triggers {
        pollSCM('H/1 * * * *')
    }

    stages {
        stage('Checkout Code') {
            steps {
                checkout scm
            }
        }

        stage('Verify GitHub Changes') {
            steps {
                echo 'SUCCESS: Jenkins fetched the latest GitHub code!'
                echo 'Project: DevOps'
                echo 'Repository: Gaushik2008/devops'
                echo 'Branch: main'
                echo "Build Number: ${BUILD_NUMBER}"
            }
        }

        stage('Build Status') {
            steps {
             echo 'AUTOMATIC POLLING VERIFIED - TEST 2'
            }
        }
    }

    post {
        success {
            echo 'PIPELINE RESULT: SUCCESS'
        }

        failure {
            echo 'PIPELINE RESULT: FAILED'
        }
    }
}
