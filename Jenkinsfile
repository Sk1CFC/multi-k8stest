pipeline{
  agent any
  parameters{
    string(name: 'BRANCH_NAME')
    string(name: 'SLEEP_TIME')
    string(name: 'APP_PORTS')
  }
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
        echo "${params.SLEEP_TIME}"
        echo "${env.PATH}"
        echo "${env.TEST}"
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
