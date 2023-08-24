pipeline {
    agent any

    environment {
        DIRECTORY_PATH = "https://github.com/jbm1412/sit753-week5-jenkins.git"
        TESTING_ENVIRONMENT = "Week 5 Testing Environment"
        PRODUCTION_ENVIRONMENT = "Manonarayanan Janardhan Bhagavathi"
    }

    stages {
        stage("Build") {
            steps {
                echo "fetch the source code from the directory path specified by the environment variable"
                echo "compile the code and generate any necessary artifacts"
            }
        }
        stage("Test") {
            steps {
                echo "unit tests"
                echo "integration tests"
            }
        }
        stage("Code Quality Check") {
            steps {
                echo "check the quality of the code"
            }
        }
        stage("Deploy") {
            steps {
                echo "deploy the application to a testing environment specified by the environment variable"
            }
        }
        stage("Approval") {
            steps {
                sleep(10)
            }
        }
        stage("Deploy to Production") {
            steps {
                echo "deploying the code to ${PRODUCTION_ENVIRONMENT}"
            }
        }
    }
}