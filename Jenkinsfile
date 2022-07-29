pipeline{
    agent any
    stages{
        stage("COMPILE"){
            
            steps{
                script{
                    echo "Compiling the code"
                }
            }
        }
        stage("UNITTEST"){
            
            steps{
                script{
                    echo "Testing the code"
                    
                }
            }
            
        }
         stage("PACKAGE"){
             
             steps{
                script{
                    echo "Packaging the code"
                    
                }
            }
        }
         stage("DEPLOY"){
            
            steps{
                script{
                    echo "Deploying the app"
                }
            }
        }
    }
}
