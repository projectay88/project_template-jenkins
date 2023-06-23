pipeline {
    agent {
        label 'master-node'
    }
    triggers {
            cron('H/3 * * * *')
        }
    stages {
        withCredentials([usernamePassword(credentialsId: 'dockerhub_pass', usernameVariable: 'projectay889', passwordVariable: '112233gT!')]
        stage ('docker hub') {
                steps{
                sh '''docker login -u $USERNAME -p $PASSWORD'''
                }
            }
        
          }
      }

