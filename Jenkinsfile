pipeline {
  agent any
  parameters {
    choice(
      name: 'Cho',
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
        sh 'python3 ${params.Cho}'
      }
    }
  }
}