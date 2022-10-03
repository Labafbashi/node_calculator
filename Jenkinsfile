pipeline {
    agent any
      stages {
        stage('PreBuild') {
          steps{
            echo 'Pre Build'
            sh "ls -la ${pwd()}"
          }
        }
        stage('Test') {
          steps{
            echo 'Test'
          }
        }
        stage('Build') {
          steps{
            echo 'Build'
          }
        }
        stage('PostBuild') {
          steps{
            echo 'Post Build'
          }
        }
    }
}
