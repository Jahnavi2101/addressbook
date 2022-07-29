pipeline{
    agent none
    tools{
        jdk 'Myjava'
        maven 'Mymaven'
    }
   
    stages{
      
        stage("Compile"){
            agent { label 'linux_slave'}
         steps{
                echo "COMPILING THE CODE"
                sh 'mvn compile'
            }
        }
        stage("UnitTest"){
            agent { label 'linux_slave'}
          steps{
                echo "Testing code"
                sh 'mvn test'
            }
            
        }
        stage("Package"){
            agent any
           steps{
             script{
                script{
                    echo "Packaging the code"
                    sh 'mvn package'
  
             }
            
              
               
            }
            
        }
    }
    }
}

