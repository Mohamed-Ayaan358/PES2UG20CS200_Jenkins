pipeline{
    agent any
    stages {
      stage('Build') {
        steps {
          sh 'g++ -o app PES2UG20CS200.cpp'
        }
      }
      stage('Test') {
        steps{
          sh './app'
        }
      }
      stage('Deploy') {
        steps {
          sh 'Its done'
        }
      }
    }
    post{
        failure{
            echo "Pipline failed"
        }
    }
}