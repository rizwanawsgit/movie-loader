node	{	
	stage('Checkout'){
		checkout scm
	}
	stage('UnitTest'){
		sh "docker build -t py-unittest-img -f Dockerfile.test ."
		sh "docker container run pyUnitTestImg"
	}
	
}
