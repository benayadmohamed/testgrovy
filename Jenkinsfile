def workspace = pwd()
pipeline {
    agent any

    parameters {
    extendedChoice(
            name: 'someName',
            description: 'dddd',
            type: 'PT_JSON',
            groovyScriptFile : "${workspace}/data"
            )
    }

    stages {
        stage('Hello') {
            steps {
                sh'ls .'
                sh "cat ${env.WORKSPACE}/data"
                echo "${env.WORKSPACE}/data"
                echo 'Hello World'
            }
        }
    }
}
