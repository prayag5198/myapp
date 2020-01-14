pipeline {
   agent any
      stages {
         stage('Build') {
            steps {
               //sh 'mvn clean package'
               bat label: '', script: 'mvn clean install'
            }
         }
         stage('Deploy') {
            steps {
               deploy adapters: [tomcat9(credentialsId: 'edc73646-e88e-4aac-a22a-48ea400dedc0', path: '', url: 'http://localhost:8180/')], contextPath: 'helloworld', war: '**/*.war'
            }
        }
    }
}
