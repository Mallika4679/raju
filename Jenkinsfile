pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        sh 'echo \'hello stage1\''
      }
    }

    stage('stage2') {
      steps {
        sh 'echo \'hello stage2\''
        git(poll: true, branch: 'main', url: 'https://github.com/Mallika4679/raju.git')
        git(url: 'https://github.com/Mallika4679/raju.git', branch: 'main', poll: true)
      }
    }

  }
}