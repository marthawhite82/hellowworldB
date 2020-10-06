pipeline {
  agent any
  tools {
    maven 'M2_HOME'
  }
  stages {
    stage('Build'){
      steps {
        sh 'mvn clean'
        sh 'mvn install'
        sh 'mvn package'
      }
    }
    stage('Test'){
      steps {
        echo "test step"
         sh 'maven test'
      }
    }
     stage('Deploy'){
      steps {
        echo "build step"
        sleep 2
      }
    }
    stage('Docker image'){
      steps {
        echo "image step"
        sleep 2
      }
    }
    
  }
}
