pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                input "Enter"
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
    }
}
