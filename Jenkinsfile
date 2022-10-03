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
    node {
    // This displays colors using the 'xterm' ansi color map.
        ansiColor('xterm') {
            // Just some echoes to show the ANSI color.
            stage "\u001B[31mI'm Red\u001B[0m Now not"
        }
    }
}
