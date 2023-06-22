pipeline {
    agent {
        label 'master-node'
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
