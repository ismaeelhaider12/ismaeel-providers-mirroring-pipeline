 pipeline {
    agent any

    stages {

stage ('Testing') {
      steps {
                script {
                    withCredentials([string(credentialsId: 'AccessKeyID', variable: 'AWS_ACCESS_KEY_ID'), string(credentialsId: 'SecretAccessKey', variable: 'AWS_SECRET_ACCESS_KEY')]) {
                    try {

                        sh "echo Credentail succeeded"
                        sh "terraform init"
                        

                    } catch (err) {
                        sh "echo failed jenkins"

                    }

                    }

                 }                     
                }
      }
        }
                                        
        }
     }
