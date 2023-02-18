pipeline{
  agent any 
  stages {
    stage('Build'){
      steps{
        sh 'cd main  && g++ working.cpp'
        echo 'Build executed successfully'
      }
    
    }
    stage('Test'){
      steps{
        sh 'cd main && ./a.out'
        echo 'Test executed successfully'
      }
    }
    stage('Deploy'){
      steps{
        echo 'Deployment executed successfully'
      }
    }
  }
  post{
    failure{
      echo 'Failure of pipeline'
    }
  }
}
