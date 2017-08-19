pipeline {
  agent any
  stages {
    stage('Greeting') {
      steps {
        echo 'Hello'
      }
    }
    stage('') {
      steps {
        input(message: 'Can i start the job', id: 'message', ok: 'yes')
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