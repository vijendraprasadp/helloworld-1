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
      parallel {
        stage('qa') {
          steps {
            echo 'Running QA Build and test'
            echo 'running buils'
            sleep(time: 5, unit: 'SECONDS')
            echo 'performing QA testing'
          }
        }

        stage('qa test') {
          steps {
            echo 'qa int testing'
            sleep 10
            echo 'qa int testing complited'
          }
        }

      }
    }

  }
}