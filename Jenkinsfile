pipeline {
    agent any
    node {
      ansicolor('xterm'){
        stage "\u001B[31mI'm Red\u001B[0m Now not"
      }
      stages {
        stage('PreBuild') {
          steps{
            echo 'Pre Build'
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
}
