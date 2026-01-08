pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
      }
    }

    stage('Test stages') {
      parallel {
        stage('Test stages') {
          steps {
            echo 'Running Tes2'
          }
        }

        stage('Test1') {
          steps {
            echo 'Running Test1'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployment completed'
        input(message: 'Are you sure to deploy?', ok: 'Yes, I am sure.')
      }
    }

    stage('Notify for new  build') {
      steps {
        echo 'New build comleted'
      }
    }

  }
}