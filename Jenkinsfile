pipeline
{
  agent any
  stages
  {
    stage("GIT")
    {
      steps
      {
        git branch: 'main', url: 'https://github.com/Sathiyan2002/task05.git'
      }
    }
    stage("CLEAN")
    {
      steps
      {
       sh "mvn clean"
      }
    }
    stage("INSTALL")
    {
      steps
      {
        sh "mvn install"
      }
    }
    stage("SHELLSCRIPT")
    {
      steps
      {
        git branch: 'feature', url: 'https://github.com/Sathiyan2002/task05.git'
        sh "bash shell.sh"
      }
    }
  }
}
