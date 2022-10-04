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
  post{
    always{
      discordSend description: "Discord Notifier with Jenkins file", footer: "EC Utbildning", link: env.BUILD_URL, result: currentBuild.currentResult, title: JOB_NAME "MH Labaf", webhookURL: "https://discordapp.com/api/webhooks/1016232403573952522/hTI450pJEORFpFXYs3YG9JpedNCEGYnb1exf93xNyUj7mvC04L5M6Q-Fm2W2sEas8HcI"
    }
  }
}
