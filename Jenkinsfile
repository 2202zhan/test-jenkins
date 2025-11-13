pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Клонируем проект...'
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Собираем проект...'
            }
        }
        stage('Run') {
            steps {
                echo 'Запускаем Python код...'
                bat 'python main.py'
            }
        }
    }
}
