node('MVN'){
    
    stage('GIT'){
        git branch: 'Dev', url: 'https://github.com/sandeep5683/game-of-life.git'
    }
    stage('Build'){
        sh 'mvn install'
    }
    stage(Dummy'){
        sh 'pwd'
    }
	stage('dummy'){
	    sh 'pwd'
	}
    stage('Archive'){
        archiveArtifacts 'gameoflife-web/target/*.war'
        junit 'gameoflife-web/target/surefire-reports/*.xml'
    }
}