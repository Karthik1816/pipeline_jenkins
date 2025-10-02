pipeline {
    agent any

    

    stages {
        stage('Checkout'){
            steps {
                git url: 'https://github.com/Karthik1816/pipeline_jenkins.git', 
                    branch: 'main', 
                    credentialsId: 'app_git' 
            }
        }

        stage('Prallel Stages') {
                stage('Check code quality repo1'){
                    steps {
                        sh '''
                            pwd 
                            ls -lrt
                            exit 1
                        '''
                    }
                }

                stage('Build'){
                    steps {
                        sh '''
                            pwd 
                            ls -lrt
                            sleep 10
                        '''
                    }
                }
            }
        }

        stage('stage_final') {
            steps{
                echo "This is final stage"
            }
        }
      
    }

}