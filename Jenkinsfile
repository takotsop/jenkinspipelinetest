pipeline {
  agent any
  stages {
    stage('git remote') {
      steps {
        sh '''#!/bin/bash

mkdir jenkinstestpipeline

cd jenkinstestpipeline

git remote add origin https://github.com/takotsop/jenkinspipelinetest.git

sleep 2s

'''
      }
    }
    stage('branch') {
      steps {
        sh '''#!/bin/bash

git checkout -b tanner

'''
      }
    }
    stage('truffle init') {
      steps {
        sh '''#!/bin/bash

truffle init

sleep 5s'''
      }
    }
    stage('add branch') {
      steps {
        sh '''#!/bin/bash

git add .

sleep 5s

git commit -m "testing"'''
      }
    }
    stage('push') {
      steps {
        sh '''#!/bin/bash

git push origin tanner'''
      }
    }
  }
}