node {
    node(corp-apis-dev-hlg) {
        stage("Deploy ${envKeyUpperCase}") {
            checkout scm
            sh "hostname"
            cleanWs()
        }
    }
}
