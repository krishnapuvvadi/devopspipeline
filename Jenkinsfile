pipeline {
agent any
stages {
    stage (build) {
        steps {
            echo 'build processing step done'
          }
        }
     stage (deploy) {
         steps {
             echo 'deploy step'		 
        }
    }
    stage (testing) {
        steps {
            echo 'testing step succeeded'
        }
    } 
    stage (plan) {
        steps {
            echo 'planning done';
            bat 'ipconfig'
        }
    }
}
    post {
        always {
            cleanWs()
        }
        failure {
            echo 'only if job fails'
        }
        success {
            echo 'only if job successfully completed'
        }
    }
   }
