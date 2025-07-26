@Library('my_shared_library') _
pipeline{
    agent any

    stages{

        stage('Git Checkout'){
            steps{
                gitCheckout(
                    branch: "main",
                    url: "https://github.com/VIJAYKUMAR-96/vg_devops_java_app.git"
                )             
            }
        }
        stage('Unit Test Maven'){
            steps{
                script{
                    sh 'mvn test'
                }            
            }
        }
    }
}