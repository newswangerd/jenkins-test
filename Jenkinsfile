pipeline {
  agent { docker 'williamyeh/ansible:centos7' }
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
