pipeline {
  agent { docker { image 'python:3.10.0' } }
  stages{
    stages("build"){
      steps{
        script{
        sh 'pip install flask'
        }
        }   
    }
    stages("test"){
      steps{
        script{
        sh 'python test.py'
        }
        }
    }
    stages("deploy"){
      steps{
        script{
        echo "DEPLOYING NOW"
        }
        }
    }
  }
}
