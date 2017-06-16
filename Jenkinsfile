pipeline {
  agent { docker 'williamyeh/ansible:centos7' }
  environment {
    HOME = '/tmp'
  }
  stages {
    stage('test'){
      steps {
        sh 'su'
        sh 'pwd'
        sh 'ls'
        sh 'python test.py'
        sh 'printenv'
        sh 'ansible-playbook playbook.yml'
      }
    }
  }
}
