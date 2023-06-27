pipeline {
    agent {
        label 'debian'
    }
    triggers {
            cron('H/3 * * * *')
        }
    stages {
	stage ('git install') {
		steps {
		sh 'sudo apt install git'
		      }
			      
                                     }
    stages {
        stage ('docker install') {
        steps {
        sh 'sudo apt-get update; sudo apt-get install ca-certificates curl gnupg'
                }

            }

        }
        
           }
}
