pipeline {
    agent any
    stages {
	stage('Launch launcher') {
	    steps {
	    	sh 'uname -a'
		sh 'alias python=python3 && python --version'
		sh 'python3 --version'		
		sh 'python python/dronelauncher_python.py &'
		sh 'sleep 60 ; exit'	
            }
	}
    }
}
