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
            
           }
}
