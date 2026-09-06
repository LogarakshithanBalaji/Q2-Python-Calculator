pipeline {
    agent any

    options {
        skipDefaultCheckout(true)
    }

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/LogarakshithanBalaji/Q2-Python-Calculator.git'
            }
        }

        stage('Build') {
            steps {
                bat '(echo 10 & echo 5 & echo +) | python calculator.py'
            }
        }

    }
}