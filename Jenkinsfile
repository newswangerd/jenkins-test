pipeline {
  agent any
  environment {
    HOME = '/tmp'
  }
  stages {
    stage('test'){
      steps {
        ansiblePlaybook("./playbook.yml")
      }
    }
  }
}
