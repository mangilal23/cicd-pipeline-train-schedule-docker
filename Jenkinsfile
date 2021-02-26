pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Running build automation'
                sh './gradlew build --no-daemon'
                archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
        Stage("Docker Image Creation"){
            when {
            branch 'master'
            }
            steps{
                script {
                
                }
            }
        }
    }
}
