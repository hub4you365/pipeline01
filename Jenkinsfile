node('slave'){
  stage('build'){
    sh 'make ID=${BUILD_ID} -f Makefile.docker build'  
  }
}
