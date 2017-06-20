pipeline {
  agent any
  environment {
    HOME = '/tmp'
  }
  stages {
    stage('test'){
      steps {
        ansiblePlaybook("./playbook.yml")
        sh "echo $GIT_PREVIOUS_SUCCESSFUL_COMMIT"
      }
    }
  }
}
