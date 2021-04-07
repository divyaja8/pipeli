pipeline {
    agent none

    stages {
        stage('stage 1') {
		    agent { label 'master'}
            steps {
				echo "this is stage one "
				 sh 'sleep 05'
            }
        }
		
		stage('stage 2') {
		agent { label 'slave1'}
            steps {
                echo "this is stage two"
				sh 'sleep 05 '
       
            }
        }
	    stage('stage 3') {
		agent { label 'master'}
            steps {
				echo "this is stage one "
				 sh 'sleep 05'
            }
        }
		stage('stage 4') {
		agent { label 'slave1'}
            steps {
				echo "this is stage one "
				 sh 'sleep 05'
            }
        }
		
	}
}
