pipeline {
  agent any
  stages {
    stage('Build test') {
      steps {
        sh 'echo " building ... "'
      }
    }
    stage('test firefox ') {
      parallel {
        stage('test firefox ') {
          steps {
            sh '''echo "test firefox " 
date'''
          }
        }
        stage('test chrome ') {
          steps {
            sh '''echo " test chrome " 
date 
'''
          }
        }
        stage('test edge') {
          steps {
            sh '''echo " test edge" 
date'''
          }
        }
        stage('test IE') {
          steps {
            sh '''test "IE" 
date '''
          }
        }
      }
    }
    stage('deploy') {
      steps {
        sh 'echo " deploy" '
      }
    }
  }
}