pipeline {
  agent any
  environment {
    HOME = '/tmp'
  }
  stages {
    stage('test'){
      steps {
        sh "echo $GIT_COMMIT"
        ansiblePlaybook("./playbook.yml")
      }
    }
  }
}
