
pipeline {
    agent any

    parameters {
    extendedChoice(
            name: 'someName',
            description: 'dddd',
            type: 'PT_JSON',
            groovyScriptFile : "${pwd()}/data"
            )
    }

    stages {
        stage('Hello') {
            steps {
                sh'ls .'
                sh "cat ${pwd()}/data"
                echo "${pwd()}/data"
                echo 'Hello World'
            }
        }
    }
}
