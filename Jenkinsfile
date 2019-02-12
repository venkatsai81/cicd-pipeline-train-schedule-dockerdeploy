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
    agent none 
    stages {
        stage('Example Build') {
            agent { docker 'maven:3-alpine' } 
            steps {
                echo 'Hello, Maven'
                sh 'mvn --version'
            }
        }
        stage('Example Test') {
            agent { docker 'openjdk:8-jre' } 
            steps {
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
}

