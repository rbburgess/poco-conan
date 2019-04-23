@Library('poco-shared-libs')_
import com.poco.GlobalVars

pipeline {
    agent any
    environment {
        IS_UNIX = GlobalVars.isUnix()
    }
    stages{
        stage("Building"){
            steps{
               echo 'Hello World'
               sayHello 'Steve'
            }
        }
        stage("Deply"){
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