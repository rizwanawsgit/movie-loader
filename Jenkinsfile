node{
  stage('checkout'){
	  checkout scm
  } 
  stage('Unit Test'){
	sh "docker build -t ${imageName}-test -f Dockerfile.test ."
	sh "docker run --rm ${imageName}-test"
    }
}
