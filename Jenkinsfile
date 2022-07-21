@Library('piper-lib-os') _
node() {
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
    stage('build') {
        print("In the build Step")
        mtaBuild script: this
  }
  stage('deploy') {
    cloudFoundryDeploy script: this
  }
}
