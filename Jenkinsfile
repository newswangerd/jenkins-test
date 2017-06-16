pipeline {
    agent { docker 'williamyeh/ansible:centos7' }
    stages {
      stage('test'){
        sh 'ansible-playbook playbook.yml'
      }
    }
}
