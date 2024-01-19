pipeline {
    agent any

    stages {
        stage('Build') {
            steps {    
                // Запуск Jenkins Job для сборки и загрузки 
                build job: 'Build-And-Upload', wait: true
            }
        }
        stage('Deploy') {
            steps {
                // Запуск Jenkins Job для деплоя с помощью Ansible
                build job: 'Deploy-With-Ansible', wait: true
            }
        }
    }
}