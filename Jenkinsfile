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
            echo 'testing step'
        }
    }  
}
}
