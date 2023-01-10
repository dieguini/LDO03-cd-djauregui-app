pipeline{
    agent{
        docker {
            image "openjdk:17-jdk-alpine3.14"
        }
    }
    stages{
        stage("Start"){
            steps{
                echo "========executing First========"
            }
            post{
                always{
                    echo "========always========"
                }
                success{
                    echo "========A executed successfully========"
                }
                failure{
                    echo "========A execution failed========"
                }
            }
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}