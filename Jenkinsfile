node {
  stage('SCM') {
    git "https://github.com/Kathirsindhu/pipeline.git"
  }
  stage('SonarQube Analysis') {
    def scannerHome = tool 'SonarScanner';
    withSonarQubeEnv() {
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}
