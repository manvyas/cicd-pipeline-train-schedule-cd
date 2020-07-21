pipeline {
   agent any
     stages {
        stage('Build') {
            steps {
               ws("C:/manu") {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
  }
}
