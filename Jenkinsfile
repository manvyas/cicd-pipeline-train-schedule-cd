pipeline {
     agent {
       node {
        label 'my-defined-label'
        customWorkspace 'C:/workspace'
      }
     }
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
