pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                powershell '''
                    Copy-Item index.html -Destination C:\\jen\\ -Force
                    Stop-Website -Name "testJenkins"
                    Start-Website -Name "testJenkins"
                '''
            }
        }
    }
}
