node {
    stage('Compile') {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '23bbab93-73bd-422f-8a2a-7a45f13a44fe', url: 'https://github.com/christophmarckx/devops-jenkins']]])
    }
    stage('Test') {
        junit ''
    }
    stage('Proceed?') {
        milestone()
        input message: "Proceed?"
        milestone()
        echo 'Proceed?'
    }
    stage('Finished') {
        echo 'Finished'
    }
}