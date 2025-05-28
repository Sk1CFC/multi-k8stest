pipeline{
  agent any
  //options {
    //skipDefaultCheckout()  // Prevents automatic full checkout
  //}
  tools{
    maven 'M399'
  }
  stages{
    //agent{ label 'mymachine' }
    stage('Build'){
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
