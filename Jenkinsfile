node	{	
	stage('Checkout'){
		checkout scm
	}
	stage('UnitTest'){
		"sudo docker.build("py-unittest-img -f Dockerfile.test .")"
		 py-unittest-img.inside{
			"python test_main.py"
		}
	}
	
}
