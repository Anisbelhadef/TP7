pipeline {
  agent any
  stages{

  stage('test') {
       steps{
          bat './gradlew test'
          archiveArtifacts 'build/test-results/test/*.xml'
       }
   }


}
}