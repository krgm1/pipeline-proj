pipeline {
	agent master
	stages {
		stage('---clean---'){
			steps {
				tool name: 'mvn 3.6.1', type: 'maven'
				sh "mvn clean"
			}
		}
		stage('---test---') {
			steps {
				tool name: 'mvn 3.6.1', type: 'maven'
				sh "mvn test"
			}
		}
		stage('---package---'){
			steps {
				tool name: 'mvn 3.6.1', type: 'maven'
				sh "mvn package"
			}
		}
	}
}
