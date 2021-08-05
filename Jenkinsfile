node
{
  echo "Github branch name ${env.BRANCH_NAME}"
      def mavenHome = tool name: "maven"
    stage('checkout')
    {
        git credentialsId: '9141c2a7-bcc0-4f97-8bde-24e0df0b6f3e', url: 'https://github.com/HAREESH1817/maven-standalone-application.git'
    }
    stage('build')
    {
        sh "${mavenHome}/bin/mvn clean package"
    }
}
