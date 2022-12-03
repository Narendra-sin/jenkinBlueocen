pipeline {
  agent any
  stages {
    stage('Fetch Code') {
      steps {
        git(url: 'https://github.com/Narendra-sin/jenkinBlueocen.git', branch: 'devops')
      }
    }

    stage('Install Apache') {
      steps {
        sh 'sudo apt install apache2 -y'
      }
    }

    stage('Deployment') {
      steps {
        sh 'sudo cp -R * /var/www/html/'
      }
    }

  }
}