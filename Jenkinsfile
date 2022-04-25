pipeline {
    agent any 

    stages ('CI') {
        stage ('checkout') {
          steps {
              echo 'checkout'
              checkout scm 
          }  
        }

        stage ('Build') {
         steps {
              //script
              sh 'mvn clean package'
          }  
        }

        stage ('Test') {
          steps {
              //script
              echo 'Test'
              sh 'mvn test'
            }  
        }
    }
}

