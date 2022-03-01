node{
  stage('checkout'){
	  checkout scm
  } 
  stage('Unit Test'){
	  docker build -t myimage -f Dockerfile.test .
	  docker run --rm myimage python test_main.py
    }
}
