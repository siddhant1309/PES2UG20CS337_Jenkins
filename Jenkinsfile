pipeline{
  agent any
  stages{
  stage('Build') {
    steps{
      sh 'g++ -o PES2UG20CS337 PES2UG20CS337.cpp'
    }
  }

  stage('Test') {
    steps{
       sh './PES2UG20CS337'
    }
  }

  stage('Deploy') {
    steps{
      echo 'DEPLOYMENT SUCCESSFUL'
    }
  }
  }

  post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}