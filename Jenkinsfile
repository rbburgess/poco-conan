pipeline {
    agent any
    stages{
        stage("Building"){
            steps{
               if(isUnix()){
                   echo "Unix"
               } else{
                   echo "Windows"
               }
            }
        }
        stage("Testing"){
            steps{
                echo "Testing"
            }
        }
    }
}