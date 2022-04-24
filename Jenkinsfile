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
     scrept{
       def imageTest= sudo docker.build("${imageName}-test","-f Dockerfile.test .")
       imageTest.inside{
         sh 'sudp python test_main.py'
     }
   }
   }
 }
  }
}
