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
                sh "cat ${workspace}/data"
                echo "${workspace}/data"
                echo 'Hello World'
            }
        }
    }
}
