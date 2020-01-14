pipeline {
   agent any
    stages {
        stage('Build') {
            steps {
               //sh 'mvn clean package'
               bat label: '', script: 'mvn clean install'
            }
        }
    }
}
