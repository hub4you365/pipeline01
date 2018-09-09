node('slave'){
    
    sh 'id'
    
    docker.image('openjdk:8u171-jdk-alpine').inside(){
        sh 'java -version'
    }
    
}
