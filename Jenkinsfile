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
                // Используем полный путь к python.exe
                bat '"C:\\Python310\\python.exe" main.py'
            }
        }
    }
}
