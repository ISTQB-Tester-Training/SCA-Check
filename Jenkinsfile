pipeline {
    agent any

    stages {
        stage('SCM') {
            steps {

                git 'https://github.com/ISTQB-Tester-Training/StaticCodeanalysis-Showcase-Template.git'
            }
        }
        
        stage('Code Analysis') {
            steps {

                sh "mvn sonar:sonar -Dsonar.host.url=http://ctp-tester-training.tk:30002/"
            }
        }
    }
}