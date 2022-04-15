#!/usr/bin/env groovy

pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        echo 'Hello world!'
      }
    }
    stage('Checkout') {
      steps {
        scm Checkout
      }
    }
    stage('Run Scritps') {
      steps {
        def workspace = pwd ()
        echo workspace
        def externalMethod = load("execute-command.groovy")
        externalMethod.proc()
      }
    }
  }
} 