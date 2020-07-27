node{
    def mvnHome
    stage('Initiate tests on BrowserStack'){
        browserstack(credentialsId: 'new key', localConfig: [localOptions: '', localPath: '']) {
             sh 'mvn test -P local'
        }
    }
}
