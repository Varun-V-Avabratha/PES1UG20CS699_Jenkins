pipeline {
  agent any
  stages {
    stage('Build') {
      steps{
        sh '-o task5_PES1UG20CS699 task5.cpp'
        echo 'Build Stage is Successful'   
      }
    }
    
    stage('Test'){
      steps{
        sh './task5_PES1UG20CS699'
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
