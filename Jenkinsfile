@Library('my_shared_library') _
pipeline{
    agent any

    stages{

        stage('Git Checkout'){
            steps{
                gitCheckout(
                    branch: "main",
                    url: "https://github.com/VIJAYKUMAR-96/shared_library.git"
                )             
            }
        }
        stage('Unit Test Maven'){
            steps{
                script{
                    mvnTest()
                }            
            }
        }
    }
}