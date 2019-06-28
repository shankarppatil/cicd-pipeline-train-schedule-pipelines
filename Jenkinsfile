pipeline{
  agent any
  stages
  {
    stage "build"
      steps "archive"
      {
        echo "build started"
        ssh ./gradlew build --no-daemon
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
  }
}


