pipeline {
    agent any
    //environment { 
        //BROWSERSTACK_USERNAME = 'nithyamani3'
        //BROWSERSTACK_ACCESS_KEY = 'P4JKysg5WuchQxBfKQu1'
    //}
    stages {
        stage('Test') {
            browserstack(credentialsId: 'new key', localConfig: [localOptions: '', localPath: '']) {
                steps {
                    sh 'mvn test -P single'
                }
            }
        }
    }
}
