pipeline {
  agent any
  
  triggers {
    pollSCM('H/5 * * * *')  
  }

  stages {
    stage('Checkout') { steps { checkout scm } }
    stage('List files') { steps { sh 'pwd && ls -la' } }
    stage('Build (placeholder)') { steps { echo 'No build step needed for this repo' } }
    stage('Test (placeholder)') { steps { echo 'No tests defined' } }
    stage('Quality (placeholder)') { steps { echo 'No linters configured' } }
    stage('Package (placeholder)') { steps { echo 'Nothing to package' } }
    stage('Deploy (placeholder)') { steps { echo 'No deployment for this task' } }
  }

  post {
    success { echo 'Build succeeded.' }
    failure { echo 'Build failed.' }
  }
}
