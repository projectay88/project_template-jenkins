pipeline {
    agent {
        label 'master-node'
    }
    triggers {
            cron('H/3 * * * *')
        }
    stages {
        stage ('docker hub') {
                steps {
                sh """
                docker ps -a
                """
                }
                             }
        
           }
      }
