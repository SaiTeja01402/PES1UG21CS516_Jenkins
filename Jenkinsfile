pipeline {
  agent any

  stages{
    stage('Build'){
      steps{
        script{
          sh 'g++ -o executable main/PES1UG21CS516.cpp'
        }
        echo 'Build Stage Successful'
      }
  }
    
  stage('Test'){
    steps{
      script{
        sh './executable'
      }
      echo 'Test Stage Successful'
    }
  }
    
Stage('Deploy'){
  steps{
    echo 'Deployment Successful'
  }
}
}

post{
  failure{
    echo 'Pipeline failed'
  }
}
}
    
