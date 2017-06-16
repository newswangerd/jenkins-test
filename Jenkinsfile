pipeline {
  agent { docker 'williamyeh/ansible:centos7' }
  stages {
    stage('test'){
      steps {
        sh 'ansible-playbook playbook.yml'
      }
    }
  }
}
