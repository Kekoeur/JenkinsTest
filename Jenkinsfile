pipeline {

  agent any

  stages {
  stage('build') {
    steps {
      echo 'Building'
    }
  }

  stage('test') {
    steps {
        composer install
        ./vendor/bin/phpunit
    }
  }

  stage('deploy') {
    steps {
        echo 'Deploying ...'
        echo 'Done'
    }
  }
 }
}