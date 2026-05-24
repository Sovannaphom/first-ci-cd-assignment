pipeline {
    agent any
    stages {
        stage("Testing "){
            steps{
                sh """
                    ls -lrt 

                    cd ansible && ansible -i inventory.ini testing-server -m ping 
                     
                """
                dir('ansible'){
                    step{
                        sh """
                            ls -lrt 
                         """
                    }
                }
            }
        }


     
    
       
        
    }
}
