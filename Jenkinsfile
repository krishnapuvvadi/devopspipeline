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
             echo 'deploy step is done'		 
        }
    }
    stage (testing) {
        steps {
            echo 'testing step is completed'
        }
    }  
}
}
