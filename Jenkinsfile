pipeline {
  agent any
  stages {
    stage('Build test') {
      steps {
        sh '''echo " building ... "
echo `date`
sleep 1'''
      }
    }
    stage('test ') {
      parallel {
        stage('test firefox ') {
          steps {
            sh '''echo "test firefox " 
echo `date `
sleep 1 '''
          }
        }
        stage('test chrome ') {
          steps {
            sh '''echo " test chrome " 
echo `date`
sleep 1'''
          }
        }
        stage('test edge') {
          steps {
            sh '''echo " test edge"
exit 1 
echo `date`
sleep 1 '''
          }
        }
        stage('test IE') {
          steps {
            sh '''test "IE" 
echo `date `
sleep 1 
'''
          }
        }
      }
    }
    stage('deploy') {
      steps {
        sh '''echo " deploy" 
echo `date`
sleep 1 '''
      }
    }
  }
}
