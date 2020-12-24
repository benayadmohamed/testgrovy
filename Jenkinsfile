
pipeline {
    agent any

    parameters {
    extendedChoice(
            name: 'someName',
            description: 'dddd',
            type: 'PT_JSON',
            groovyScript : '''
            GroovyShell shell = new GroovyShell()
            def tools = shell.parse(new File('./data.groovy'))
             return tools.jsonEditorOptions
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
