node('slave'){
  stage('check out'){
    git 'https://github.com/hub4you365/pipeline01'
  }
  stage('build docker'){
    docker.build("${BUILD_ID}", "-f Dockerfile.build .").inside() {
      sh 'node -v'  
    }
  }
}


