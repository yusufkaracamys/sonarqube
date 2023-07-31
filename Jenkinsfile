pipeline {
        agent none
        
        stages {
          stage("build & SonarQube analysis") {
            agent any
            steps {
                sh 'java Main.java'
            }
          }
        }
      }
