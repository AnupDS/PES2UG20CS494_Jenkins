pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh 'g++ PES2UG20CS494.cpp -o PES2UG20CS494'
      }
    }
   
    stage('Test') {
      steps {
        sh './PES2UG20CS494'
      }
    }
   
    stage('Deploy') {
      steps {
       sh '/departent/services'

    }
  }
 
  post {
    failure {
       
          echo 'Pipeline failed'
        }
    }
   
  }
