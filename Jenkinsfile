pipeline {
  agent any
  stages {
    stage('testrpc') {
      steps {
        sh '''#!/bin/bash

mkdir tanner

testrpc &

sleep 2s
'''
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