node {
    stage('Compile') {
        checkout scm
            grdl('compileJava')
    stage('Test') {
        grdl('test')
    }
    stage('IntegrationTest') {
        grdl('IntegrationTest')
    }
    def grdl(task){
    println "gradlew ${task}""
    }
    dir('dev'){
    sh "./gradlew ${task} --info --stacktrace"
    }
        echo 'Finished'
    }
}