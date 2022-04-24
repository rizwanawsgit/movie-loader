pipeline{
  agent any
  stages{
    stage('checkout'){
      steps{
        checkout scm
      }
  }
 stage('Unit Tests'){
   steps{
     sudo docker.build("imagetest -f Dockerfile.test .")
     sudo imagetest.inside{
       sh 'python test_main.py'
   }
   }
 }
  }
}
