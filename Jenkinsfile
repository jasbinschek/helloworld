pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
    stage('Cloning Git') {
      steps {
        git 'https://github.com/jasbinschek/helloworld.git'
      }
    }
    stage('Install dependencies') {
      steps {
        sh 'npm install'
      }
    }
     
    stage('Test') {
      steps {
         sh 'npm test'
      }
    }  

    stage('Deploy') {
      steps {
         echo 'Deploy Sucess'
      }
    }      
  }
}
