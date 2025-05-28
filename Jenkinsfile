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
        sleep "time: ${params.SLEEP_TIME}, unit: 'SECONDS'"
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
