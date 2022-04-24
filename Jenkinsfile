node	{	
	stage('Checkout'){
		checkout scm
	}
	stage('UnitTest'){
		sh "docker build -t pyUnitTestImg -f Dockerfile.test ."
		sh "docker container run pyUnitTestImg"
	}
	
}
