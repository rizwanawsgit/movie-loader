node	{	
	stage('Checkout'){
		checkout scm
	}
	stage('UnitTest'){
		def Home=/var/lib/jenkins/workspace/python
		sh '$Home python test_main.py'
	}
}
