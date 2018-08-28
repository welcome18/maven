def workspace;
node ('EC2')
  {
      stage('checkout')
      {
          checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/welcome18/maven.git']]])
          workspace =pwd()
      }
      stage('Static Code Analysis')
      {
          echo "Static Code Analysis"
      }
      stage('Build')
      {
          echo "Build The Code"
      }
      stage('Unit Testing')
      {
          echo "Unit Testing"
      }
      stage('Delivery')
      {
          echo "Delivery"
      }
  }
