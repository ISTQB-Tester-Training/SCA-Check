pipeline {
    agent any

    stages {
        stage('SCM') {
            steps {

                git 'https://github.com/ISTQB-Tester-Training/SCA-Check.git'
            }
        }

        stage('Code Analysis') {
            steps {

                sh "mvn sonar:sonar -Dsonar.host.url=http://ctp-tester-training.tk:30002/"
            }
        }
    }
}