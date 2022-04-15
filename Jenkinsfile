#!/usr/bin/env groovy

pipeline {
  agent any
  def workspace = pwd ()
  def externalMethod = load("execute-command.groovy")
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
        echo workspace
        externalMethod.proc()
      }
    }
  }
} 