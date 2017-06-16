pipeline {
  agent { docker 'williamyeh/ansible:centos7' }
  stages {
    stage('test'){
      steps {
        sh 'pwd'
        sh 'ls'
        sh 'python test.py'
        sh 'mkdir test'
        sh 'ansible-playbook playbook.yml'
      }
    }
  }
}
