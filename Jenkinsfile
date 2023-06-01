pipeline{
  agent any
  
  stages{
    stage('install'){
      steps{
        sh 'npm install'
      }
    }
    
    stage('source-code-import'){
      steps{
        git branch: 'main', changelog: false, poll: false, url: 'https://github.com/akshit4/project_fitness_app'
      }
    }
    
    stage('build'){
      steps{
        sh 'npm start'
      }
    }
  }
}
