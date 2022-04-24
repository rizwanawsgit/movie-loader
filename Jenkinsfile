node{
  stage('Checkout'){
    checkout scm
}
  stage('Unit Tests'){
    def imageName = 'mlabouardy/movies-loader'
    def imageTest= docker.build("${imageName}-test", "-f Dockerfile.test .")
    imageTest.inside{
      sh 'python test_main.py'
}
}
