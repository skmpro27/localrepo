pipeline {
  agent any
  parameters {
    choice(
      name: 'choice',
      choices: ['main.py', 'app.py', 'tests.py'],
      description: 'Passing the Environment'
    )
  }
  stages {
    stage('version') {
      steps {
        sh 'python3 --version'
      }
    }
    stage('hello') {
      steps {
        sh 'python3 tests.py'
      }
    }
  }
}