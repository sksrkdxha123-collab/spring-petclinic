pipeline {
 agent any
  
 tools {
    jdk 'JDK21'
    maven 'M3'
 }
 
 stages {
     stage('Git Clone') {
         steps {
             git url: 'https://github.com/sksrkdxha123-collab/spring-petclinic.git',
             branch: 'main'
         }
     }
     stage('Maven Build') {
         steps {
             sh 'mvn clean package -Dmaven.test.failure.ignore=true'
         }
     }
     stage('Docker Image Create') {
         steps {
             echo 'Docker Image Create'
         }
     }
     stage('Dokcer Hub Login') {
         steps {
             echo 'Dokcer Hub Login'
         }
     }
     stage('Docker Image Push') {
         steps {
             echo 'Docker Image Push'
         }    
     }
     stage('Dokcer Container Run') {
         steps {
             echo 'Dokcer Container Run'
         }
     }
 }
}
