pipeline {
    agent any

    stages {
        stage('build') {
            steps {

                lastChanges since: 'LAST_SUCCESSFUL_BUILD', format:'LINE', matching: 'LINE'
                echo 'Hello World'
                script {
                    env.changes = lastChanges()
                }
                sh 'env'
            }
        }

        stage('deploy') {
            steps {
                echo 'Hello World'
                sh 'env'
            }
        }

    }
}
