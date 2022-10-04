pipeline {
    agent any
    parameters {
      string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
    }
      stages {
        stage('PreBuild') {
          steps{
            echo 'Pre Build'
            sh "ls -la ${pwd()}"
          }
        }
        stage('Test') {
          steps{
            echo "${params.Greeting} World!!!"
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
