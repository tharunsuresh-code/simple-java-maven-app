pipeline {
  agent {
    docker {
      image 'sebastianj1w/maven_with_git'
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