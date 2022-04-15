#!/usr/bin/env groovy

node {
    stage('Checkout') {
    echo "${BRANCH_NAME} ${env.BRANCH_NAME}"
    scm Checkout
    }
    
    stage('Test') {
        steps {
        echo 'Hello world!'
        def workspace = pwd()
        def externalMethod = load("execute-command.groovy")
        echo workspace
        externalMethod.proc()
        }
    }

} 