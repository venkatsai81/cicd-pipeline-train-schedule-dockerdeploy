/*pipeline {
    agent any
    stages {
        stage('Build') {
      
              steps {
                echo 'twooooooooo'
                //sh './gradlew build --no-daemon'
                //archiveArtifacts artifacts: 'dist/trainSchedule.zip'
            }
        }
         
    }
}*/
pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
              echo 'This is build stage'
            }
        }
        stage('Test') { 
            steps {
               echo 'This is Test stage'
            }
        }
        stage('Deploy') { 
            steps {
               echo 'This is deployment pages'
            }
        }
    }
}
