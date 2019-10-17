node('MVN') {
    stage('Git'){
        git branch: 'dev', url: 'https://github.com/sandeep5683/game-of-life.git'
    }
    stage('Build'){
        sh label: '', script: 'mvn package'
    }

}