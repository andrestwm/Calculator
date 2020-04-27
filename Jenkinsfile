node{
	stage('SCM Checkout'){	
		git 'https://github.com/andrestwm/Calculator'
	}
	stage('Compile-Package'){
		//Get maven home path
		
		def mvnHome = tool name: 'MAVEN_3.6.3', type: 'maven'
		sh "${mvnHome}/bin/mvn package"
	}
}
