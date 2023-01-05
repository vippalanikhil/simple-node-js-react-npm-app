pipeline {
  agent any
  environment {
    CI = 'true'
  }
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/vippalanikhil/simple-node-js-react-npm-app.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
        sh 'npm cache clean --force'
        sh 'npm i --force'
        sh 'npm run build'
      }
    }  
  }
}
