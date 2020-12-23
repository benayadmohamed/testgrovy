pipeline {
    agent any

    parameters {
    extendedChoice(
            name: 'someName',
            description: 'dddd',
            type: 'PT_JSON',
            groovyScriptFile : "/var/snap/jenkins/1687/workspace/testpp/data"
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
