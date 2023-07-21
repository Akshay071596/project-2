pipeline{
        agent{
             label{
                  label"built-in"
             }
        }

  stages{
         stage("stage-1"){
                      steps {
                            sh"yum install httpd -y"
                            sh "service httpd start"
                      
                      }
           
         }

      stage("stage-2"){
             agent{
                    label{
                          label"slave-1"
                          
                    }
             }
           steps{
                 sh "sudo yum install git -y"
           }
      }

      stage("stage-3"){
             agent{
                    label{
                          label"slave-2"
                          
                    }
             }
           steps{
                 sh "sudo yum install git -y"
           }
      }

        stage("stage-4"){
             agent{
                    label{
                          label"slave-3"
                          
                    }
             }
           steps{
                 sh "sudo yum install git -y"
           }
      }
  }
}
