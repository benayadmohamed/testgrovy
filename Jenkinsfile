
pipeline {
    agent any

    parameters {
    extendedChoice(
            name: 'someName',
            description: 'dddd',
            type: 'PT_JSON',
            groovyScript : '''
            evaluate(new File("./data.groovy"))
            '''
            //groovyScriptFile : "${env.WORKSPACE}/data"
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
