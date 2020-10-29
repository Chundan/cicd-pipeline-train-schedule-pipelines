pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                echo 'start building...'
                sh './gradlew clean build' 
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }

    }
}
