node{
    stage('Initiate tests on BrowserStack'){
        browserstack(credentialsId: 'new key', localConfig: [localOptions: '', localPath: '']) {
            withEnv(['BROWSERSTACK_USERNAME=' + user]) {
                sh label: '', returnStatus: true, script: '''#!/bin/bash -l
                                     mvn test -P local
                                   '''
            }
        }
        junit testDataPublishers: [[$class: 'AutomateTestDataPublisher']], testResults: 'target/surefire-reports/TEST-*.xml'
    }
}
