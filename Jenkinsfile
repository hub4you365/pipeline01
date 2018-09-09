node('slave'){
  stage('check out'){
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/hub4you365/pipeline01.git']]])
  }
  stage('build docker'){
    docker.build("${BUILD_ID}", "-f Dockerfile.build .").inside() {
      sh 'node -v'  
    }
  }
}
