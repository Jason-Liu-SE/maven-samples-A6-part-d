pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/Jason-Liu-SE/maven-samples-A6-part-d.git', branch: 'main')
      }
    }

    stage('run') {
      steps {
        sh '''mvn clean
mvn test
mvn verify'''
      }
    }

  }
  tools {
    maven 'DHT_MVN'
    jdk 'DHT_SENSE'
  }
}
