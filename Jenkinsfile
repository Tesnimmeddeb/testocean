pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
      }
    }

    stage('Test') {
      parallel {
        stage('Test2') {
          steps {
            echo 'Running Test2'
          }
        }

        stage('Test1') {
          steps {
            echo 'Running Test1'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deplyment completed'
      }
    }

  }
}