pipeline {
 agent any
  stages {
      stage('Pull') {
         steps {
             git 'https://github.com/pranathi16/ctsdemoproject.git'
         }
      }
      stage('Package') {
         steps {
            bat 'mvn package'
         }
      }
      stage('Execute') {
         steps {
            bat 'java -jar "C:/programdata/Jenkins/.jenkins/workspace/job5/target/cts1-1.0-SNAPSHOT.jar"'
         }
      }
   }
}
