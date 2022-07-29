pipeline{
    agent none
    tools{
        jdk 'myjava'
        maven 'mymaven'
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
            agent any
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

