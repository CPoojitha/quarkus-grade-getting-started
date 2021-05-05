pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
               
               bat 'mvn -Dmaven.test.failure.ignore=true clean package'
               }
               }
               
               
       stage('Building image') {
            steps{
                
          bat 'docker build -f Dockerfile -t quarkus/hello-world-jvm .'
            }
            }
            
            
            
        }
        }