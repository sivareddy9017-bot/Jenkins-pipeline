pipeline {
    agent {
        node {
          label 'Java'
        }
    }
    environment {
     course="Jenkins"
    }
    options {
          disableConcurrentBuilds()  //we should not run parallel builds for this option
          timeout(time: 5, unit: 'SECONDS') // Pipeline build process check
    }

    stages {
        stage('Build') {
            steps {
                script {
                    sh """
                      echo "This is build"
                      echo $course
                      sleep 5
                    """
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
    }
    //post build
    post {  
         always{
            echo "pipeline executed"
         }
    }
}


