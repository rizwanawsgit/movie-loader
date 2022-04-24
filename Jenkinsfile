node	{	
	stage('Checkout'){
		checkout scm
	}
	stage('UnitTest'){
		sh "sudo docker build -t py-unittest-img -f Dockerfile.test ."
		sh "sudo docker container run pyUnitTestImg"
	}
	
}
