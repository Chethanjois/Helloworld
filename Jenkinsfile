def call (body) 
{
def config = [:]
body.resolveStrategy = Clousre.DELEGATE_FIRST
body.delegate = config
body()

pipeline {
  agent any
  stages {
    stage('Build') {
      script {
        sh 'ls -ltr'  
      }
    }  
  }
}

}
