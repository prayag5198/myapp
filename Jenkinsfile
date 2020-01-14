pipeline {
   agent any
    stages {
        stage('Build') {
            steps {
               //sh 'mvn clean package'
               set M2_HOME =  C:\Program Files\Apache Software Foundation\apache-maven-3.6.3
               set path =  C:\Program Files\Apache Software Foundation\apache-maven-3.6.3\bin:%path%;
               bat label: '', script: 'mvn clean install'
            }
        }
    }
}
