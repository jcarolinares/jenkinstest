pipeline{
  agent any
  environment{
    PROGRAM_NAME="helloworld.py"
  }


  stages {
    stage('Compile Stage'){

      steps {
          script{
          checkout scm
          sh 'echo "Compile stage"'
          sleep 10
          }
      }
    }

    stage('Testing stage'){
      steps {

          sh 'echo "Testing stage"'
          sh 'python $PROGRAM_NAME'
      }
    }

    stage('Deployment stage'){
      steps {
          sh 'echo "Deployment stage"'


      }
    }

  }


}
