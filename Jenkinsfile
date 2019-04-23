pipeline {
    agent any
    
    stages{
        stage("Building"){
            steps{
               script {
                   if(isUnix()){
                    echo "Unix"
                    } else{
                        echo "Windows"
                    }
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