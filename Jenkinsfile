pipeline {
    agent any
    stage('Maven Build & Test') {
	steps {
	    sh 'python python/dronelauncher.py'
        }
    }
    
    post {
        always {
            junit '**/TEST*.xml'
            emailext attachLog: true, attachmentsPattern: '**/TEST*xml',
	    body: 'Bod-DAy!', recipientProviders: [culprits()], subject:
            '$PROJECT_NAME - Build # $BUILD_NUMBER - $BUILD_STATUS!'
	}
    }
}
