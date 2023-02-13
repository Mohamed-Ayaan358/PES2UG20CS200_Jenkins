pipeline{
    agent any
    stages {
      stage('Build') {
        steps {
          sh 'g++ -o app source.cpp'
        }
      }
      stage('Test') {
        steps
          sh './app'
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