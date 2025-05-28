pipeline{
  agent any
  //options {
    //skipDefaultCheckout()  // Prevents automatic full checkout
  //}
  tools{
    maven 'M399'
  }
  stages{
    stage('Build'){
      steps{
        echo "Building....."
        bat "timeout /t ${params.SLEEP_TIME} /nobreak"
      }
    }
    stage('Test'){
      steps{
        echo "Testing....."
        sh "echo "testing on port ${params.PORT_NO}""
      }
    }
    stage('Deploy'){
      steps{
        echo "Deploying....."
      }
    }
  }
}
