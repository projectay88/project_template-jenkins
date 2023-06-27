pipeline {
    agent {
        label 'master-node'
    }
    triggers {
            cron('H/3 * * * *')
        }
    stages {
        stage ('docker install') {
                steps {
                sh "sudo apt-get update; sudo apt-get install ca-certificates curl gnupg"
                }
                             }
        
           }
      }
