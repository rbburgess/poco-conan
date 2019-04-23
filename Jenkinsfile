@Library('poco-shared-libs')_
import com.poco.GlobalVars

pipeline {
    agent any
    stages{
        stage("Building"){
            steps{
               echo 'Hello World'
               mkdir -p build
            }
        }
        stage("Deploy"){
            steps {
                echo env.IS_UNIX
            }
        }
        stage("Testing"){
            steps{
                echo env.IS_UNIX
            }
        }
    }
}