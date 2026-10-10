
pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Gaushik2008/devops.git'
            }
        }

        stage('Hello') {
            steps {
                echo 'THE NAME IS GAUSHIKKKK'
            }
        }
         stage('One') {
            steps {
                echo 'THE NAME IS OPTIMUS'
            }
        }
    }
}
