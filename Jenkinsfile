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
                withCredentials([usernamePassword(credentialsId: 'dockerhub_pass', usernameVariable: 'projectay889', passwordVariable: '112233gT!')]

                sh """
                docker login -u $USERNAME -p $PASSWORD
                """
                }
                             }
        
           }
      }
