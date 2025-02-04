pipeline {
    agent any 

    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/I-am-saiprasad/Jenkins-Zero-To-Hero.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'        
            }
        }

        stage('Run Tests') {
            steps {
                sh 'pytest test_app.py'
            }
        }
    }
}

