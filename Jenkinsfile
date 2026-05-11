pipeline {
    agent any

    tools {
        maven 'Maven'
        jdk 'JDK21'
    }

    stages {

        stage('Git Checkout') {
            steps {
                git branch: 'main',
                url: 'https://github.com/Meghana-km-05/lab61.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

    }
}
