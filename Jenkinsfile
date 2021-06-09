def buildNumber = env.BUILD_NUMBER as int
if (buildNumber > 1) milestone(buildNumber - 1)
milestone(buildNumber)

node {
    node(corp-apis-dev-hlg) {
        stage("Deploy ${envKeyUpperCase}") {
            checkout scm
            sh "hostname"
            cleanWs()
        }
    }
}
