node{
  stage('checkout'){
	  checkout scm
  } 
  stage('Unit Test'){
	def path = "C:\jenkinshomedirectory\workspace\movie-loader_develop"
	sh '$path python test_main.py'
    }
}
