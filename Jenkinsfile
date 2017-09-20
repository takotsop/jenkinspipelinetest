pipeline {
  agent any
  stages {
    stage('make working directory') {
      steps {
        sh '''#!/bin/bash
mkdir tannertest
cd tannertest
truffle init

sleep 5s'''
      }
    }
    stage('no') {
      steps {
        sh '''#!/bin/bash

git commit -m "new files"

sleep 5s'''
      }
    }
    stage('git add') {
      steps {
        sh '''#!/bin/bash

git push origin master

sleep 10s'''
      }
    }
  }
}