def imageName = 'mlabouardy/movies-loader'
node{
  stage('checkout'){
	  checkout scm
  } 
  stage('Unit Test'){
	def imageTest = docker.build("${imageName}-test", "-f Dockerfile.test .")
	sh "docker run --rm -v $PWD/reports:/app/reports ${imageName}-test"
	junit "$PWD/reports/*.xml"		
  }
}
