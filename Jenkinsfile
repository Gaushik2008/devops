pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                checkout([
                    $class: 'GitSCM',
                    branches: [[name: '*/main']],
                    userRemoteConfigs: [[
                        credentialsId: 'Github',
                        url: 'https://github.com/Gaushik2008/devops.git'
                    ]]
                ])
            }
        }

        stage('Hello') {
            steps {
                echo 'Automatic Build Test'
            }
        }
    }
}
