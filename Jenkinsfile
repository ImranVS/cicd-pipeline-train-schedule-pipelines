pipeline {
  agent any
  stage {
    stage{build} {
      stage {
        echo 'running build automation'
        sh './gradlw build --no=demon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
