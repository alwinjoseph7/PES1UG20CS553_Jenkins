pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        sh 'g++ -o task5 task5_code.cpp'
        build job: 'PES1UG20CS553-1'
      }
    }
    stage('Test'){
      steps{
        sh './task55'
      }
    }
   stage('Deploy'){
      steps{
        echo 'Deploying'
      }
    }
  }
  post{
    failure{
      echo 'Pipeline failed'
    }
  }
}
