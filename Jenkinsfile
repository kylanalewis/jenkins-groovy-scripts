#!/usr/bin/env groovy

node {
    stage('Checkout') {
    checkout scm
    }
    
    stage('Test') {
        echo 'Hello world!'
        def workspace = pwd()
        echo workspace
    }

    stage('Execute Job') {
        def externalMethod = load("executeCommand.groovy")
        externalMethod.method()
    }

    stage('Cleanup') {
        deleteDir()
    }

} 