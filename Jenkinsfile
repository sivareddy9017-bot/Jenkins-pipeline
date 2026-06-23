pipeline {
    agent {
        node {
          label 'Java'
        }
    }

    stages {
        stage('Build') {
            steps {
                script {
                    sh """
                      echo "This is build"
                    """
                }
            }
        }
    }
        stage('Test') {
            steps {
                script {
                    sh """
                       echo "This is test"
                    """
            }
        }
    }

    post {
         always{
            echo "pipeline executed"
         }
    }
}

