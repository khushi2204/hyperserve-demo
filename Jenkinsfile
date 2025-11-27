pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/khushi2204/hyperserve-demo.git'
            }
        }

        stage('Run Script') {
            steps {
                sh '''
                    echo "Running script inside Linux Jenkins"
                    chmod +x print_status.sh
                    ./print_status.sh
                '''
            }
        }
    }
}
