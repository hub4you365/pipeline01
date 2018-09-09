node('slave'){
    
    sh 'id'
    
    docker.image('openjdk:8u181-jdk').inside(){
        sh 'java -version'
    }
    
}
