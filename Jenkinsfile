pipeline{

  agent any

  tools{
    maven 'Mave 3.6.3'
  }

  stages{
    stage('build'){
      steps{
        mvn compile
      }
    }
    stage('test'){
      steps{
        mvn clean test
      }
    }
    stage('package'){
      steps{
        MVN package -DskipTests
      }
    }
  }

}
