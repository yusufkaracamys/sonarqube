pipeline {
        agent any
        tools { 
        maven 'Maven 3.3.9' 
        jdk 'jdk17' 
    }
        stages {
          stage("build & SonarQube analysis") {
            agent any
            steps {
                sh 'java Main.java'
            }
          }
        }
      }
