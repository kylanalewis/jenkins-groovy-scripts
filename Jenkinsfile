#!/usr/bin/env groovy

node {
    stage('Checkout') {
    scm Checkout
    }
    
    stage('Test') {
        steps {
        echo 'Hello world!'
        def workspace = pwd()
        def externalMethod = load("executeCommand.groovy")
        echo workspace
        externalMethod.proc()
        }
    }

} 