pipeline {
    agent any
    
    stages {
    
    stage('Git') {
      steps {
        git 'https://github.com/arth20/devops_calculator'
      }
    }
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh './scripts/test.sh'
            }
        }
       
    }
}
