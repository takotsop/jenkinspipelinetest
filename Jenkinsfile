pipeline {
  agent any
  stages {
    stage('make working directory') {
      steps {
        sh '''#!/bin/bash
mkdir tannertest
cd tannertest

git remote add origin git@github.com/takotsop/jenkinspipelinetest.git
sleep 2s
truffle init

sleep 5s'''
      }
    }
    stage('commit') {
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