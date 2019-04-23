@Library('poco-shared-libs')_

pipeline {
    agent any
    
    stages{
        stage("Building"){
            steps{
               echo 'Hello World'
               sayHello 'Steve'
            }
        }
        stage("Testing"){
            steps{
                echo "Testing"
            }
        }
    }
}