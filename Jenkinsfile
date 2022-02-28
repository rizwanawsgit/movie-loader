def imageName = 'mlabouardy/movies-loader'
node{
  stage('checkout'){
    checkout scm
  } 
  stage('Unit Test'){
    def customImage = docker.build("my-image:${env.BUILD_ID}", "-f Dockerfile.test .")
    customImage.inside{
      bat 'python test_main.py'
	}
    }
}
