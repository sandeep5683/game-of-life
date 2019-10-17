node('MVN') {
    stage('Git'){
        git branch: 'dev', url: 'https://github.com/sandeep5683/game-of-life.git'
    }
    stage('Build'){
        sh label: '', script: 'mvn install'
    }
    stage('Archive'){
        archive 'gameoflife-web\\target\\*.war'
        junit 'gameoflife-web\\target\\surefire-reports/*.xml'
    }
	stage('dummy'){
	      sh 'pwd'
	}
}