pipeline {
	agent any

	stages {
		stage('Buiding') {
			steps {
				echo 'Buiding'
			}
		}
		stage('Deploy') {
            when {
              expression {
                currentBuild.result == null || currentBuild.result == 'SUCCESS' 
              }
            }
            steps {
                sh 'make publish'
            }
        }
		stage('Deploying') {
			steps {
				echo 'Deploying'
			}
		}
	}
}