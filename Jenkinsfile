node()
{
  stage 'checkout'
  deleteDir()
  checkout scm
  sh "rm -f *.deb"
  stage 'build'
  sh "make deb"
  stage 'publish'
  sh "make publish-deb"
}
