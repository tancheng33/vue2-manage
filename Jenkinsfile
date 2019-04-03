pipeline {
  agent any
  stages {
    stage('build') {
      agent {
        node {
          label 'node'
        }

      }
      steps {
        node(label: '1')
        build(propagate: true, wait: true, job: '1111')
      }
    }
  }
}