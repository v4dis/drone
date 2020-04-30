pipeline {
    agent any
    stages {
	stage('Launch launcher') {
	    steps {
	    	sh 'uname -a'
		sh 'python python/dronelauncher_python.py &'
		sh 'sleep 60 ; exit'	
            }
	}
    }
}
