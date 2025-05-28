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
        echo "${params.BRANCH_NAME}"
        echo "Building....."
        bat "timeout /t ${params.SLEEP_TIME} /nobreak"
      }
    }
    stage('Test'){
      steps{
        echo "Testing....."
        echo "testing on port ${params.APP_PORT}"
      }
    }
    stage('Deploy'){
      steps{
        echo "Deploying....."
      }
    }
  }
}
