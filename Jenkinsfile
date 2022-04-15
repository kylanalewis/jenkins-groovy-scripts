#!/usr/bin/env groovy

node {
    stage('Checkout') {
    checkout scm
    }
    
    stage('Test') {
        echo 'Hello world!'
        def workspace = pwd()
        def externalMethod = load("executeCommand.groovy")
        echo workspace
    }

    stage('Cleanup') {
        deleteDir()
    }

} 