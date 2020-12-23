pipeline {
    agent any

    parameters {
    extendedChoice(
            name: 'someName',
            description: 'dddd',
            type: 'PT_JSON',
            groovyScriptFile : 'data.groovy'
            )
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
