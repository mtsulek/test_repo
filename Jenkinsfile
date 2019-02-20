pipeline {
    agent {
        node {
            label 'LS'
        }
    }

    parameters {
        params.SLEEP_TIME_IN_SECONDS = 100
    }

    stages{
        stage ("wait_prior_starting_smoke_testing") {
            def time = params.SLEEP_TIME_IN_SECONDS
            echo "Waiting ${SLEEP_TIME_IN_SECONDS} seconds for deployment to complete prior starting smoke testing"
            sleep time.toInteger() // seconds
        }
    }
}