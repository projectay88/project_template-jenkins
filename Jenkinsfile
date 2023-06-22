pipeline {
    agent {
        label 'master-node'
    }
    stages {
        stage('create docker image') {
            steps {
                echo "docker image"
                dir ('.'){
                        sh 'docker build .'
                    }
              }
          }
      }
  }
