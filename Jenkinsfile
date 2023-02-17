pipeline {
  agent any
  stages {
    stage('Build') {
      steps{
        sh 'g++ -o task5 task5.cpp'
        echo 'Build Stage is Successful'   
      }
    }
    
    stage('Test'){
      steps{
        sh './task5'
        echo 'Test Stage is Successful'
      }
    }
    
    stage('Deploy'){
      steps{
        echo 'Deploy Stage is Successful'
      }
    }
    
  }
  
  post{
    failure{
      echo 'Pipeline Failed'
    }
  }
  
}
