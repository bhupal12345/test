currentBuild.displayName = "online-shopping-#"+currentBuild.number
pipeline {
    agent any

    

    stages {
        stage('---clean---') {
          steps {
            sshagent(['te'])   {
           
sh "scp -o StrictHostKeyChecking=no /var/lib/jenkins/workspace/teste/* ec2-user@35.178.203.42:/home"
              
                
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
