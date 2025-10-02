pipeline {
  agent any
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
            echo "BEAUTY world"
            sh '''
               ls
               pwd
            '''
        }
    }
  }
}
