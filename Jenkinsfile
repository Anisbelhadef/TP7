pipeline {
  agent any
  stages{
  stage('build') {
   steps{
      bat './gradlew build'
      archiveArtifacts 'build/libs/*.jar'
   }
   }
   }
}