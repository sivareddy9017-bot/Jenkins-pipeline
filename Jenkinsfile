pipeline {
    agent {
        node {
          label 'Java'
        }
    }
    environment 
     course=Jenkins
    
    stages {
        stage('Build') {
            steps {
                script {
                    sh """
                      echo "This is build"
                      echo $course
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
    post {  
         always{
            echo "pipeline executed"
         }
    }
}


