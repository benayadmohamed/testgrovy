pipeline {
    agent any

    parameters {
    extendedChoice(
            name: 'someName',
            description: 'dddd',
            type: 'PT_JSON',
            groovyScriptFile : "${env.WORKSPACE}data"
            )
    }

    stages {
        stage('Hello') {
            steps {
                sh'ls .'
                echo 'Hello World'
            }
        }
    }
}
