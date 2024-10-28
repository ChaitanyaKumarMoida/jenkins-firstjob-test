pipeline {
    agent any

    stages {
        stage('Parallel Stages') {
            parallel {
                stage ('stage 1') {
                    steps {
                        echo 'Running stage 1'
                    }
                }
                stage ('stage 2') {
                    steps {
                        echo 'Running satge 2'
                    }
                }
                stage ('stage 3') {
                    steps {
                        echo 'Running stage 3'
                    }
                }
            }
        }
    }
}
