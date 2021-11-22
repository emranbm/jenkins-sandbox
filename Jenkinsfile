pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
                publishHTML (target : [allowMissing: false,
                 alwaysLinkToLastBuild: true,
                 keepAll: true,
                 reportDir: 'reports',
                 reportFiles: 'myreport.html',
                 reportName: 'My Reports',
                 reportTitles: 'The Report'])
            }
        }
    }
}
