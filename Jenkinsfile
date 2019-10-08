node{
	stage('SCM Checkout'){
		git 'https://github.com/krgm1/pipeline-proj'
	}
	stage('Compile-Package'){
		// Get maven home path
		def mvnHome = tool name: 'Maven 3.6.1', type: 'maven'
		sh "${mvnHome}/bin/mvn package"
	}
}
