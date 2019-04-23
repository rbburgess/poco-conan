@Library('poco-shared-libs')_
import GlobalVars

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
                GlobalVars.isUnix
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