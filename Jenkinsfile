pipeline{
        agent{
             label{
                  label"slave-2"
                  customWorkspace "/mnt/assignment -2"
             }
        }
  stages{
         stage("stage-1"){
                      steps {
                            sh" sudo yum install httpd -y"
                            sh "sudo service httpd start"
                      
                      }
           
         }
        stage("stage-2"){
                        steps{
                                sh "sudo chmod -R 777 /var/www/html "
                                sh "sudo cp index.html /var/www/html"
                        }
        }


     
        
  }
}
