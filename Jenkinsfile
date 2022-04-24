pipeline{
  agent any
  stages{
    stage('checkout') {
      steps {
        checkout scm
      }
    }
 stage('Unit Tests'){
   steps{
     "sudo docker build -t imagetest -f Dockerfile.test ."
     "sudo docker run imagetest"
   }
 }
  }
}
