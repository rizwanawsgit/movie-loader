node{
  stage('checkout'){
	  checkout scm
  } 
  stage('Unit Test'){
	  def Dockerfile = "Dockerfile.test"
	  def customImage = docker.build("my-image, -f $Dockerfile .")
	  customImage.inside{
		  bat "python test_main.py"
	}
    }
}
