@Library('common')

def init = new com.minted.pipeline.Initializer()
def shellRunner = new com.minted.pipeline.ShellRunner(this)
def defaultNode = new com.minted.config.JenkinsConfig().get('defaultNode')
def minted_node = new com.minted.pipeline.MintedNode()

minted_node.mintedGlobalNode(defaultNode, shellRunner) {
  stage('Sample') {
    println("Global checks should have run before this!")
  }
}
