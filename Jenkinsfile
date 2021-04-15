pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'Running Maven build '
        sh 'mvn clean package'
      }
    }

    stage('qa') {
      steps {
        echo 'Running QA Build and test'
        echo 'running buils'
        sleep(time: 5, unit: 'SECONDS')
        echo 'performing QA testing'
      }
    }

  }
}