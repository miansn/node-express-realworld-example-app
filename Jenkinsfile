node {
    env.NODEJS_HOME = "${tool 'Node 6.x'}"
    // on linux / mac
    env.PATH="${env.NODEJS_HOME}/bin:${env.PATH}"
    // on windows
    env.PATH="${env.NODEJS_HOME};${env.PATH}"
    sh 'npm --version'

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
