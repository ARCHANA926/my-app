pipeline {
  agent any
  stages{
    stage("SCM checkout"){
      steps {
         git credentialsId: 'slave-ssh', url: 'https://github.com/ARCHANA926/my-app.git' branch: "master"
       }
      stage("maven build"){
        steps {
          sh "clean packaage"
            }
      }
  }
}
