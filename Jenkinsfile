pipeline{
    agent any

    stages{
          stage("Build"){
            steps{
            echo "Running Build Automation"
            sh './gradlew build --no-daemon'
    }
          }

          stage("Archive Artifacts")
          {
            steps{
            echo "Archiving Artifacts"
            archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        }
      }
    }
}
