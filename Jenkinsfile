pipeline {
  agent none
  stages {
    stage("build") {
        agent { label "slave16" }
        steps { 
            echo "HEllo world"
            sh "ls"
        }
    }
    stage("TEst") {
        agent { label "slave18"}
        steps { 
            echo "HEllo world"
            sh '''
               ls
               pwd
            '''
        }
    }
  }
}
