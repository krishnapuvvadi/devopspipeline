properties([pipelineTriggers([githubPush()])])
pipeline {
agent any
stages {
    stage (build) {
        steps {
            echo 'build step'
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
            echo 'planning done'    
        }
    }   
    post {
        always {
            echo 'always to be executed once job completed'
        }
    }   
}
}
