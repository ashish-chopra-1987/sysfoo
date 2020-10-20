pipeline{
  agent any
  steps{
    stage('build'){
      steps{
        echo 'compile maven app'
        sh 'mvn compile'
      } 
    }
  }
  steps{
    stage('test'){
      steps{
        echo 'test maven app'
        sh 'mvn clean test'
      } 
    }
  }
  steps{
    stage('package'){
      steps{
        echo 'package maven app'
        sh 'mvn package -DskipTests'
      } 
    }
  }
}
