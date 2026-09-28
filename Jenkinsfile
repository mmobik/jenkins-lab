pipeline {
    agent any

    stages {
        stage('Тестовый пайплайн') {
            steps {
                echo "ФИО: Ощепков Сергей Алексеевич"
                script {
                    docker.image('maven:3.9-eclipse-temurin-17').inside {
                        sh 'mvn -v'
                    }
                }
            }
        }
    }
}