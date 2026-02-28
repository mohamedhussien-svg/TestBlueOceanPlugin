pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building Project'
      }
    }

    stage('Testing') {
      parallel {
        stage('Testing') {
          steps {
            echo 'Test1'
          }
        }

        stage('Testing2') {
          steps {
            echo 'Testing2'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying Application'
        input(message: 'Are You Sure', ok: 'Yes Sure')
      }
    }

  }
}