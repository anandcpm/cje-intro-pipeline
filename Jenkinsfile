pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${MY_NAME}!"
        sh 'java -version'
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PWD}"
      }
    }
  }
  environment {
    MY_NAME = 'Anand'
    TEST_USER = credentials('test-user')
  }
}