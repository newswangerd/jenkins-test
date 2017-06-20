pipeline {
  agent any
  environment {
    HOME = '/tmp'
  }
  stages {
    stage('test'){
      steps {
        echo $JENKINS_URL
        ansiblePlaybook("./playbook.yml")
      }
    }
  }
}
