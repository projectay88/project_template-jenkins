pipeline {
    agent {
        label 'master-node'
    }
    triggers {
            cron('H/3 * * * *')
        }
    stages {
        stage('clear alpine') {
            steps {
                echo "clear alpine"
                sh 'docker images'
              }
          }
      }
  }
