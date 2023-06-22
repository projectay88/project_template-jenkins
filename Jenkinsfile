pipeline {
    agent {
        label 'master-node'
    }
    triggers {
            cron('H/3 * * * *')
        }
    stages {
        stage ('docker hub') {
                steps{
                withCredentials([usernamePasword(credentialsId: 'dockerhub_pass', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')])
                sh 'docker -u projectay889 -p 112233gT!'
                echo "!!!!docker login!!!!"
                }
            }
        
          }
      }

