pipeline {
  agent any
  stages {
    stage('testrpc') {
      steps {
        sh '''#!/bin/bash

testrpc &

sleep 2s

mkdir tanner'''
      }
    }
    stage('test') {
      steps {
        sh '''#!/bin/bash

truffle test'''
      }
    }
  }
}