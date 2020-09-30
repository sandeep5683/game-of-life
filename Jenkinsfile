node('MVN'){
    
    stage('GIT'){
        git branch: 'Dev', url: 'https://github.com/sandeep5683/game-of-life.git'
    }
    stage('Build'){
        sh 'mvn package'
    }
	stage('Archive){
	    archive 'gameoflife-web/target/*.jar'
	}
}