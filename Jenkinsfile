pipeline {
    agent any
    stages{
        stage("Building"){
            steps{
                echo System.properties['os.name'].toLowercase()
            }
        }
        stage("Testing"){
            steps{
                echo "Testing"
            }
        }
    }
}