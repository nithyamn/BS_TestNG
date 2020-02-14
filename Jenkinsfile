pipeline {
    agent { docker { image 'maven:3.3.3' } }
    environment { 
        BROWSERSTACK_USERNAME = 'nithyamani3'
        BROWSERSTACK_ACCESS_KEY = 'P4JKysg5WuchQxBfKQu1'
    }
    stages {
        stage('build') {
            steps {
                sh 'mvn test -P single'
            }
        }
    }
}
