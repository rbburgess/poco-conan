@Library('poco-shared-libs')_
import com.poco.GlobalVars

pipeline {
    agent any
    environment {
        IS_UNIX = 'true'
    }
    stages{
        stage("Building"){
            steps{
               echo 'Hello World'
               sayHello 'Steve'
            }
        }
        stage("Deploy"){
            steps {
                echo env.IS_UNIX
            }
        }
        stage("Testing"){
            steps{
                echo "Testing"
            }
        }
    }
}