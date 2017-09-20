pipeline {
  agent any
  stages {
    stage('testrpc') {
      steps {
        sh '''#!/bin/bash

touch dockerfile

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