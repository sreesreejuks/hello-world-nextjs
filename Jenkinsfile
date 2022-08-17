pipeline {
    agent {
        docker {
            image 'node:lts' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
		    sh 'yarn lint'
                sh 'yarn install' 
            }
        }
    }
}
