@Library('poco-shared-libs')_
import com.poco.GlobalVars

pipeline {
    agent any
    stages{
        stage("Building"){
            steps{
               echo 'Hello World'
               bat 'mkdir build'
               bat 'cd build'
               bat 'conan install ..'
               bat 'cmake .. -G "Visual Studio 15 Win64"'
               bat 'cmake --build . --config Release'
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