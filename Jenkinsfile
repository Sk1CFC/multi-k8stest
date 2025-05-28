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
        sh "sleep ${params.SLEEP_TIME}"
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
