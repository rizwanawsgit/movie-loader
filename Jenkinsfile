def ImageName = 'mlabouardy/movies-loader'
node{
  stage('checkout'){
    checkout scm
  }
  stage('Unit Tests'){
    sh "docker build -t ${ImageName}-test -f Dockerfile.test ."
    sh "docker run --rm ${ImageName}-test"
    
  }
}
