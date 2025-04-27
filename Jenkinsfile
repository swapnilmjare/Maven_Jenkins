pipeline{
  agent any;
  stages{
    stage('1'){
      steps{
        git credentialsId: 'd71b92e7-6718-4118-8587-9c79de5d66de', url: 'https://github.com/swapnilmjare/Maven_Jenkins.git'
      }
    }
  }
  post{
    success{
      sh 'tar -cvzf git.tar /var/lib/jenkins/workspace/github_pipeline'
    }
    failure{
      sh 'date'
    }
    always{
      sh 'ifconfig'
    }
  }
}
