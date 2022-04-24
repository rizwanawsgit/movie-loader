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
     sh "sudo docker build -t imagetest -f Dockerfile.test ."
     sh "sudo docker run imagetest"
   }
 }
  }
}
