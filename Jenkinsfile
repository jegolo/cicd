pipeline {
  agent {
    kubernetes {
      //cloud 'kubernetes'
      label 'mypod'
      containerTemplate {
        name 'maven'
        image 'maven:3.3.9-jdk-8-alpine'
        ttyEnabled true
        command 'cat'
      }
    }
 }
  stages { 
      stage ("Hello World") {
          steps {
              sh "echo Hello WOrld"
          }
      }
   }
}