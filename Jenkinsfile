pipeline {
  agent any
  
  stages {
    stage('git') {
          git 'https://github.com/ManashRoyINT/Dockerfile.git'
    }
    stage('print') {
          sh '''#!/bin/bash
                 echo "hello world" 
          '''
    }
    stage('docker') {
          sh '''#!/bin/bash
                docker run -d .
          '''
    }
  }
}
