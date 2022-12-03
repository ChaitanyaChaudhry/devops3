pipeline {
  agent { docker { image 'python' } }
  stages{
    stages("build"){
      steps{
        sh 'pip install flask'
      }
    }
    stages("test"){
      steps{
        sh 'python test.py'
      }
    }
    stages("deploy"){
      steps{
        echo "DEPLOYING NOW"
      }
    }
  }
}
