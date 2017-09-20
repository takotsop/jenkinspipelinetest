pipeline {
  agent any
  stages {
    stage('testrpc') {
      steps {
        sh '''#!/bin/bash

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
    stage('git commit') {
      steps {
        sh '''#!/bin/bash

git commit -m "upload files"

sleep 10s'''
      }
    }
    stage('git add') {
      steps {
        sh '''#!/bin/bash

git push origin master'''
      }
    }
  }
}