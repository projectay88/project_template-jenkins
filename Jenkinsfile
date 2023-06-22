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
                sh 'docker -u $USERNAME -p $PASSWORD'
                echo "!!!!docker login!!!!"
                }
            }
        stage('clear alpine') {
            steps {
                echo "clear alpine"
                sh 'docker build -t projectay889/my_alpine .'
                    }
              }
        stage('docker push') {
                steps {
                        sh 'docker push projectay889/my_alpine'
                    }
            }
          }
      }
  }
