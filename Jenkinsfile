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
            satge ('Unit Test') {
                steps {
                    echo 'Running Units Tests'
                }
            }
            stage ('Intregation Tests') {
                steps {
                    echo 'Running Intregation Tests'
                }
            }
            satge ('UI Test') {
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
