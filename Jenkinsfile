node	{	
	stage('Checkout'){
		checkout scm
	}
	stage('UnitTest'){
		"sudo docker build -t py-unittest-img -f Dockerfile.test ."
		"docker container run py-unittest-img"
	}
	
}
