pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-dameon'
        archieveArtifacts artifacts: 'dist/trainSchedule.zip'
    }
  }
}
