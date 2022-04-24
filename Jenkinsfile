node{
  stage('Checkout'){
    checkout scm
  }
  stage('Unit Tests'){
    def imageTest= docker.build("pythonimage -f Dockerfile.test .")
    imageTest.inside{
      sh 'python test_main.py'
}
}
