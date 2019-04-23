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
        stage("Deply"){
            when {
                isUnixSystem
            }
            steps {
                echo 'Unix'
            }
        }
        stage("Testing"){
            steps{
                echo "Testing"
            }
        }
    }
}