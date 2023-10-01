node {
  stage("code-checkout")
  {
  git credentialsId: '88cdd510-6def-4817-a0d9-f12abe24f2fa', url: 'https://github.com/DevOps-Traning/Maven-Web-Project.git'
  }
  stage("build")
  {
  def mvnHOME = tool name: 'windowsmaven', type: 'maven'
  bat "${mvnHOME}/bin/mvn clean package"
  }
  stage("build")
  {
  def mvnHOME = tool name: 'windowsmaven', type: 'maven'
  bat "${mvnHOME}/bin/mvn deploy"
  }
}
