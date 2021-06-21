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
             echo 'deploy step is completed'		 
        }
    }
    stage (testing) {
        steps {
            echo 'testing step is completed'
        }
    }  
}
}
