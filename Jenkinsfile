@Library('my_shared_library') _
pipeline{
    agent any

    stages{

        stage('git Checkout'){

            steps{

                script{
                gitCheckout(
                    branch: "main",
                    url: "https://github.com/VIJAYKUMAR-96/shared_library.git"
                )             
                }
            }
        }
    }
}