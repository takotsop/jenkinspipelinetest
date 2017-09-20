pipeline {
  agent any
  stages {
    stage('testrpc') {
      steps {
        parallel(
          "testrpc": {
            sh '''#!/bin/bash

testrpc &

sleep 2s'''
            
          },
          "mkdir": {
            sh '''#!/bin/bash

mkdir tanner'''
            
          }
        )
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