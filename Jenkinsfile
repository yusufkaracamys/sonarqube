pipeline {
        agent none
        stages {
          stage("build & SonarQube analysis") {
            agent any
            steps {
                sh 'mvn clean package sonar:sonar'
            }
          }
        }
      }
