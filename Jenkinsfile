@Library('piper-lib-os') _
node('master') {
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
}
