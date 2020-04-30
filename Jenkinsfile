pipeline {
    agent any
    stages {
	stage('Launch launcher') {
	    steps {
	    	sh 'uname -a'
		sh 'sudo apt-get update'
		sh 'python python/dronelauncher_python.py &'
		sh 'sleep 60 ; exit'	
            }
	}
    }
}
