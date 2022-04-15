#!/usr/bin/env groovy

node {
    stage('Checkout') {
    // scm Checkout
    echo " Checkout not working."
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