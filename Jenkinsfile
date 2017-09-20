pipeline {
  agent any
  stages {
    stage('git remote') {
      steps {
        sh '''#!/bin/bash

git checkout tanner


touch tanner23'''
      }
    }
    stage('add branch') {
      steps {
        sh '''#!/bin/bash

git add .

sleep 5s

git commit -m "testing jenkins"'''
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