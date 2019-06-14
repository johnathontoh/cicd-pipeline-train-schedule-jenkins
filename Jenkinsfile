pipeline {
agent any #run on any agent
stages {
 stage('Build') {
  steps {
   echo 'Running build automation'
   sh'./gradlew build --no-daemon' #daemon is a background process that speeds up build, no need for it in the pipeline
   archiveArtifacts artifacts: 'dist/trainSchedule.zip'
   }
  }
 }
}
