pipeline {
  agent {
    docker {
      image 'sanjeev3d:maven3'
        args '-v /root/.m2:/root/.m2'
    }
  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
   }
 }
}