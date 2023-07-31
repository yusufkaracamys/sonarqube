node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    def mvn = tool 'maven';
    withSonarQubeEnv() {
      sh "./gradlew sonar \
  -Dsonar.projectKey=sonarqube-test \
  -Dsonar.projectName='sonarqube-test' \
  -Dsonar.host.url=http://localhost:9000 \
  -Dsonar.token=sqp_8d3dde36cdb4aa52a906779e536cc2a386ac95ce"
    }
  }
}
