pipeline {
    agent any
    parameters {
        string description: 'private/<branch-job-name>', name: 'branch', trim: true
        string description: 'build-number', name: 'build', trim: true
    }    

    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/kiranvaltix/test'
                sh "./build.sh"
            }
        }
    }
}
