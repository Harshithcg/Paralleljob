pipeline {
  agent any
  stages {
      stage('Parallel Job') {
        parallel {
          stage('Parallel BUILD') {
            steps { 
              echo "Testing Build"
            }
    }
          stage('Parallel Build1') {
            steps { 
              echo "Testing Build1"
            }
    }
          stage('Parallel BUILD2') {
            steps { 
              echo "Testing Build2"
            }
    }
    }
      }
    stage('Parallel TEST') {
    parallel {
    stage('parallel Testing') {
      steps {
        echo "Testing on WINDOWS"
      }
    }
       stage('parallel Testing1') {
       steps {
       echo "Testing on Linux"
       }
       }
    }
  }
    stage('parallel Depoly') {
    parallel {
stage('Deploying') {
steps {
echo "Deploying in 2nd server"
}
}
stage('Deploying Image') {
steps {
echo "Deploying Image in 3rd server"
}
}
    }
    }
  }
}
