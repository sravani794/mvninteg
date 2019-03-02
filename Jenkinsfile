pipeline {
   agent any
      stages {
          stage('compile') {
                steps {
                    withMaven(maven: 'maven-3.6.0') {
                          sh 'mvn clean compile'
                      }
                  }
            }
  
            stage('testing') {
                steps {
                    withMaven(maven: 'maven-3.6.0') {
                          sh  'mvn test'
                      }
                  }
            }

            stage('install') {
                steps {
                    withMaven(maven: 'maven-3.6.0') {
                          sh 'mvn install'
                      }
                  }
            }
 
       }
 }


  

