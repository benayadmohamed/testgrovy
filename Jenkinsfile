
pipeline {
    agent node

    parameters {
    extendedChoice(
            name: 'someName',
            description: 'dddd',
            type: 'PT_JSON',
            groovyScriptFile : " ${env.WORKSPACE}/data"
            )
    }

    stages {
        stage('Hello') {
            steps {
                sh'ls .'
                sh "cat ${env.WORKSPACE}/data"
                echo " ${env.WORKSPACE}/data"
                echo 'Hello World'
            }
        }
    }
}
