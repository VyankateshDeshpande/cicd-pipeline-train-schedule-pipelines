pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				echo 'Running Build Automation'
				sh './gradlew build --no-demon'
				archiveArtifacts artifacts: 'dist/trainSchedule.zip'
			}
		}
	}
}
