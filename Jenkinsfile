pipeline {
  agent any
  stages {
    stage('') {
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