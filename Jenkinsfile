pipeline {
  agent any
  stages {
    stage('truffle init') {
      steps {
        sh '''#!/bin/bash

truffle init'''
      }
    }
    stage('testrpc') {
      steps {
        sh '''#!/bin/bash

testrpc &

sleep 2s'''
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