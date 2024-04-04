pipeline {
  agent any
  stages {
    stage('Ready') {
            steps {
             echo 'Just a beginning..'
            }
        }
    stage('version') {
      steps {
        sh 'python3 --version'
      }
    }
    stage('hello') {
      steps {
        sh 'python3 hello.py'
      }
    }
  }
   post {
        always {
            echo 'Good try, try to be better!'
        }
        success {
            echo 'Completed successfully.'
        }
        failure {
            echo 'Pipeline Failed'
        }
  }

}


