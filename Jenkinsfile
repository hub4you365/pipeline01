node('slave'){
  stage('build'){
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/hub4you365/pipeline01.git']]])
    sh 'make ID=${BUILD_ID} -f ./Makefile.docker build'  
  }
}
