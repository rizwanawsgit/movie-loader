def imageName = 'mlabouardy/movies-loader'
node{
  stage('checkout'){
    checkout scm
  }
  stage('Unit Tests'){
    sh "docker build -t ${imageName}-test -f Dockerfile.test ."
    sh "docker run --rm ${imageName}-test"
  }
}
