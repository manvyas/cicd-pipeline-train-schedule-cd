pipeline {
   agent any
     stages {
        stage('Build') {
           ws("C:/workspace") {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
  }
}
