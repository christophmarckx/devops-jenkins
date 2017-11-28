node {
    stage('This is a stage') {
        echo 'This is a stage'
    }
    stage('Another stage') {
        echo 'This is a stage'
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