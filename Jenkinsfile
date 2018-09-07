node('docker') {
    checkout scm
    stage('Build') {
        docker.image('maven').inside {
            sh 'mvn --version'
        }
    }
}