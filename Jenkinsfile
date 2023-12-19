pipeline {
  agent any
  stages{

  stage('build') {
   steps{
      bat './gradlew build'
      archiveArtifacts 'build/libs/*.jar'
   }
   }

    stage('Generate Cucumber Reports') {
               steps {
                       bat './gradlew cucumber'
               }
           }
   }
}