properties([pipelineTriggers([githubPush()])])
pipeline {
agent any
stages {
    stage (build) {
        steps {
            echo 'build processing step'
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
            echo 'always to be executed once job is completed'
        }
        failure {
            echo 'only if job fails'
        }
        success {
            echo 'only if job successfully completed'
        }
    }
}
