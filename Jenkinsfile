pipeline {
  agent any
  environment {
    HOME = '/tmp'
  }
  stages {
    stage('test'){
      steps {
        echo ${env.JENKINS_URL}
        ansiblePlaybook("./playbook.yml")
      }
    }
  }
}
