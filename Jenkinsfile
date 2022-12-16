pipeline {
    agent any
    parameters {
        string description: 'private/<branch-job-name>', name: 'branch', trim: true
        string description: 'build-number', name: 'build', trim: true
    }    

    stages {
        stage('Build') {
            steps {
                sh "./build.sh"
            }
        }
    }
}
