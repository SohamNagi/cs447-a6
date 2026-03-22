pipeline {
  agent any
  tools { 
      maven 'Maven' 
      jdk 'SDKMAN' 
  }
  stages {
    stage('CheckOut') {
      steps {
        git(url: 'https://github.com/SohamNagi/cs447-a6', branch: 'master')
      }
    }

    stage('run') {
      agent any
      steps {
        sh 'mvn verify'
      }
    }

  }
}
