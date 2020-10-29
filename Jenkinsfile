Jenkinsfile (Declarative Pipeline)
pipeline {
    stages {
        stage('check out code'){
            steps{
              checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'jenkins', url: 'https://github.com/Chundan/cicd-pipeline-train-schedule-pipelines.git']]])
            }
        }
        stage('Build') { 
            steps {
                sh './gradlew clean build' 
            }
        }

    }
}
