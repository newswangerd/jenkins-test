pipeline {
  agent { docker 'williamyeh/ansible:centos7' }
  stages {
    stage('test'){
      steps {
        sh 'python test.py'
        sh 'ansible-playbook playbook.yml'
      }
    }
  }
}
