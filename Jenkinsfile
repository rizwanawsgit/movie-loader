node{
  stage('checkout'){
	  checkout scm
  } 
  stage('Unit Test'){
	 bat 'cd C:\jenkinshomedirectory\workspace\movie-loader_develop'
	 bat '$path python test_main.py'
    }
}
