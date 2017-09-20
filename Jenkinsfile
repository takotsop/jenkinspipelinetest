pipeline {
  agent any
  stages {
    stage('git remote') {
      steps {
        sh '''#!/bin/bash

git checkout -b tanner

'''
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