pipeline {
  agent any
  stages {
    stage('Build test') {
      steps {
        sh '''echo " building ... "
echo `date`'''
      }
    }
    stage('test firefox ') {
      parallel {
        stage('test firefox ') {
          steps {
            sh '''echo "test firefox " 
echo `date `'''
          }
        }
        stage('test chrome ') {
          steps {
            sh '''echo " test chrome " 
echo `date`
'''
          }
        }
        stage('test edge') {
          steps {
            sh '''echo " test edge" 
echo `date`'''
          }
        }
        stage('test IE') {
          steps {
            sh '''test "IE" 
echo `date `'''
          }
        }
      }
    }
    stage('deploy') {
      steps {
        sh '''echo " deploy" 
echo `date`'''
      }
    }
  }
}