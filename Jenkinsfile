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
            when {
                env.IS_UNIX
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