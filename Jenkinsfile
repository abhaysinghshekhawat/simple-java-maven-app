pipeline{
  agent any
  stages{
    stage('testing'){
      steps{
        echo "hello"
        sh "pwd"
        sh "sudo cat pom.xml"
      }
      stage('testing2'){
        steps{ 
          git 'https://github.com/vimallinuxworld13/simple-java-maven-app.git'
          sh "ls"
          sh "pwd"
        }
      }
          
    }
  }
}
