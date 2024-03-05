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
        mvn clean
      }
      stage("INSTALL")
      {
      steps
      {
        mvn install
      }
       stage("SHELLSCRIPT")
    {
      steps
      {
        sh "bash shell.sh"
      }
    }
  }
}
