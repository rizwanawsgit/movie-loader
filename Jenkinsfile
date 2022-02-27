node{
  stage('checkout'){
    checkout scm
  }
  stage('Unit Tests'){
    def pythonPath=/Users/M Rizwan Ameen/AppData/Local/Programs/Python/Python39
    sh "$pythonPath python test_main.py"
  }
}
