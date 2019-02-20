pipeline {
    // agent {
    //     node {
    //         label 'LS'
    //     }
    // }

    environment {
        SLEEP_TIME_IN_SECONDS = 100
    }

    stages{
        stage("wait_prior_starting_smoke_testing") {
            steps{
                sh """
                echo "Waiting ${env.SLEEP_TIME_IN_SECONDS} seconds for deployment to complete prior starting smoke testing"
                sleep ${env.SLEEP_TIME_IN_SECONDS}
                """
            }
        }
    }
}