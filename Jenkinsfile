pipeline {
  agent any
  stages{

  stage('test') {
       steps{
          bat './gradlew test'
          archiveArtifacts 'build/test-results/test/*.xml'  // on doit le transformer a un html
          cucumber(
             buildStatus: 'UNSTABLE',
             reportTitle: 'Rapport Cucumber',
             fileIncludePattern: '**/*.json',
          )
       }
   }


}
}