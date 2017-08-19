pipeline {
  agent any
  stages {
    stage('Greeting') {
      steps {
        echo 'Hello'
      }
    }
  }
  post {
    always {
      archive 'target/**/*.jar'
      
    }
    
  }
  parameters {
    choice(choices: '''staging
prakashul-qa''', description: '', name: 'REQUESTED_ACTION')
  }
}