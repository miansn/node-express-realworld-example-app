node {

  stage('build') {
      sh 'npm --version'
      sh 'git log --reverse -1'
      sh '/usr/bin/npm install'
  }

  stage('test') {
      sh "npm test"
  }

  stage('deploy') {
      sh "npm run dev"
  }

}
