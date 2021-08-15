node {

  stage('build') {
      sh 'npm --version'
      sh '/usr/bin/npm install --no-optional'
  }

  stage('test') {
      sh "npm test"
  }

  stage('deploy') {
      sh "npm run dev"
  }

}
