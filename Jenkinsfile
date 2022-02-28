def imageName = 'mlabouardy/movies-loader'
node{
  stage('checkout'){
    checkout scm
  } 
  stage('Unit Tests'){
    bat "docker build -t ${imageName}-test -f Dockerfile.test ."
    bat "docker container run -d ${imageName}-test"
  }
}
