node(node1) {
    stage('Code clone') { 
	  git branch: 'main', credentialsId: 'git', url: 'https://github.com/suryavinay4435/jenkinsapr.git'
    }
    stage('maven version') {
	  sh 'mvn --version'
        
    }	 
    stage('code clean') {
	  sh 'mvn clean'
        
    }
     stage('code package') {
	  sh 'mvn package'   
    }
}

