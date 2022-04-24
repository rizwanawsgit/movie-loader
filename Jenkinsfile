node{
  stage('Checkout'){
    checkout scm
  }
 stage('Unit Tests'){
   def imageTest= sudo docker.build("${imageName}-test","-f Dockerfile.test .")
   imageTest.inside{
     sh 'sudp python test_main.py'
   }
 }
}
