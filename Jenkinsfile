pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Run Script') {
            steps {
                bat '"C:\\Program Files\\Git\\bin\\bash.exe" -lc "./print_status.sh"'
            }
        }
    }
}
