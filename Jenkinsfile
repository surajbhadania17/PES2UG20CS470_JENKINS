pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh 'g++ name.cpp -o name'
      }
    }
   
    stage('Test') {
      steps {
        sh './name'
      }
    }
   
    stage('Deploy') {
      steps {
         sh '/departent/services'
      }
    }
  }
 
  post {
    failure {
       
          echo 'Pipeline failed'
        }
    }
   
  }
