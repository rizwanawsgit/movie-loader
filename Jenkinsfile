def imageName = 'mlabouardy/movies-loader'
node{
  stage('checkout'){
    checkout scm
  } 
  stage('Unit Test'){
  	def imageTest= docker.build("${imageName}-test", "-f Dockerfile.test .")
	imageTest.inside{
		bat 'python test_main.py'
	}
    }
}
