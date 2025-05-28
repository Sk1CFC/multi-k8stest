pipeline{
  agent none
  //options {
    //skipDefaultCheckout()  // Prevents automatic full checkout
  //}
  tools{
    maven 'M399'
  }
  stages{
    stage('Build'){
      agent{ label 'mymachine' }
      steps{
        echo "Building....."
      }
    }
    stage('Test'){
      steps{
        echo "Testing....."
      }
    }
    stage('Deploy'){
      steps{
        echo "Deploying....."
      }
    }
  }
}
