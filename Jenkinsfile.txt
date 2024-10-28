pipeline {
    agent any

    stages {
        stage ('BUILD') {
            steps {
                echo 'Buld Repo'
            } 
        }
    stage ('TEST') {
        parallel {
            stage ('Unit Test') {
                steps {
                    echo 'Running Units Tests'
                }
            }
            stage ('Intregation Tests') {
                steps {
                    echo 'Running Intregation Tests'
                }
            }
            stage ('UI Test') {
                steps {
                   echo 'Running UI Tests' 
                }
            }
        }
    }
    stage ('DEPLOY') {
        steps {
            echo 'Deploying ....'
        }
    }
    }
}
