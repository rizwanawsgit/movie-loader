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
     sh "docker build -t imagetest -f Dockerfile.test ."
     sh "docker run imagetest"
   }
 }
  }
}
