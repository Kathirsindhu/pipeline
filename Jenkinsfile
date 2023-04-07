pipeline {
    agent any
    stages {
        stage('Pull Code From GitHub') {
            steps {
                git credentialsId: 'githubserver', url: 'https://github.com/Kathirsindhu/pipeline.git'
            }
        }
    }
}
