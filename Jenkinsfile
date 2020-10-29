pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                echo 'start building...'
                sh './gradlew clean build --no-daemon' 
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }

    }
}
