pipeline{
    agent any
    environment{
        NEW_VERSION="1.0.0"
    }
    stages{
        stage("Compile"){
            steps{
                script{
                    echo "Compiling the code"
                }
            }
        }
        stage("Test"){
            steps{
                script{
                    echo "Testing the code"
                }
            }
            post{
            always{
                echo "Testing is completed"
            }
        }
        }
        
        stage("Package"){
            steps{
                script{
                    echo "Packaging the code ${NEW_VERSION}"
                }
            }
        }
    }
}
