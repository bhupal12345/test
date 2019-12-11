currentBuild.displayName = "online-shopping-#"+currentBuild.number
pipeline {
    agent any

    

    stages {
        stage('---clean---') {
          steps {
            sshagent(['jenkins1'])   {
           
sh "scp -o StrictHostKeyChecking=no /var/lib/jenkins/workspace/teste/* jenkins1@18.130.229.211:/home"
              
                
            }
        }
        }
        stage('--test--') {
            steps {
               echo"first step1"
            }
        }
        stage('--package--') {
            steps {
              echo"first step2"
            }
        }
    }
}
