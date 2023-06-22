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
                sh 'docker -u projectay889 -p 112233gT!'
                echo "!!!!docker login!!!!"
                }
            }
        
          }
      }

